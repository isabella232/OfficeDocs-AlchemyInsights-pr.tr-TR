---
title: E-postadan sorun giderme olayları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658754"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="2a45a-102">E-postadan sorun giderme olayları</span><span class="sxs-lookup"><span data-stu-id="2a45a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="2a45a-103">Özelliğin posta kutusu için etkinleştirildiğini doğrulama: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="2a45a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="2a45a-104">Ardından ' e-postadaki etkinlikler ' günlüklerine bakın **dışarı aktarma-MailboxDiagnosticLogs <mailbox> -Component timeprofile**</span><span class="sxs-lookup"><span data-stu-id="2a45a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="2a45a-105">' E-postadaki etkinlikler ' günlüklerinde, posta kutusundaki öğeyle eşleşen ınternetmessageıd öğesini bulun.</span><span class="sxs-lookup"><span data-stu-id="2a45a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="2a45a-106">TrustScore öğenin eklenip eklenmeyeceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="2a45a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="2a45a-107">Olaylar yalnızca TrustScore = "güvenilen" olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="2a45a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="2a45a-108">TrustScore, Ileti üstbilgisindeki SPF, Vseçkim veya DMARC özellikleri tarafından belirlenir.</span><span class="sxs-lookup"><span data-stu-id="2a45a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="2a45a-109">Bu özellikleri görüntülemek için:</span><span class="sxs-lookup"><span data-stu-id="2a45a-109">To view these properties:</span></span>

<span data-ttu-id="2a45a-110">**Masaüstü Outlook**</span><span class="sxs-lookup"><span data-stu-id="2a45a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="2a45a-111">Öğeyi açma</span><span class="sxs-lookup"><span data-stu-id="2a45a-111">Open the item</span></span>
- <span data-ttu-id="2a45a-112">Dosya-> özellikleri-> Internet üstbilgileri</span><span class="sxs-lookup"><span data-stu-id="2a45a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="2a45a-113">veya</span><span class="sxs-lookup"><span data-stu-id="2a45a-113">or</span></span>

<span data-ttu-id="2a45a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="2a45a-114">**MFCMapi**</span></span>

- <span data-ttu-id="2a45a-115">Gelen kutusu 'nda öğeye gitme</span><span class="sxs-lookup"><span data-stu-id="2a45a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="2a45a-116">PR_TRANSPORT_MESSAGE_HEADERS_W arama</span><span class="sxs-lookup"><span data-stu-id="2a45a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="2a45a-117">Bu özellikler, taşıma ve yönlendirme sırasında belirlenir ve kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="2a45a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="2a45a-118">Daha fazla sorun giderme için, SPF, CıKIM ve. veya DMARC 'daki hatalar hakkında aktarım desteğiyle izlemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="2a45a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>