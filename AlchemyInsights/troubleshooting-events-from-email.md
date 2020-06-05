---
title: E-postadan Sorun Giderme Etkinlikleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569400"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="3eab2-102">E-postadan Sorun Giderme Etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="3eab2-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="3eab2-103">Posta kutusu için özelliğin etkinleştirilen olduğunu doğrulayın: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="3eab2-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="3eab2-104">Sonra 'E-posta dan Olaylar' günlükleri **İhracat-MailboxDiagnosticLogs <mailbox> -Bileşen TimeProfile** bakmak</span><span class="sxs-lookup"><span data-stu-id="3eab2-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="3eab2-105">'E-postadan Olaylar' günlüklerinde, posta kutusundaki öğeyle eşleşen InternetMessageId'i bulun.</span><span class="sxs-lookup"><span data-stu-id="3eab2-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="3eab2-106">TrustScore, öğenin ekilip eklenmediğini belirler.</span><span class="sxs-lookup"><span data-stu-id="3eab2-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="3eab2-107">Olaylar yalnızca TrustScore = "Güvenilen" ise eklenir.</span><span class="sxs-lookup"><span data-stu-id="3eab2-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="3eab2-108">Güven Puanı, İleti Üstbilgisinde bulunan SPF, Dkim veya Dmarc özellikleri tarafından belirlenir.</span><span class="sxs-lookup"><span data-stu-id="3eab2-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="3eab2-109">Bu özellikleri görüntülemek için:</span><span class="sxs-lookup"><span data-stu-id="3eab2-109">To view these properties:</span></span>

<span data-ttu-id="3eab2-110">**Masaüstü Outlook**</span><span class="sxs-lookup"><span data-stu-id="3eab2-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="3eab2-111">Öğeyi açma</span><span class="sxs-lookup"><span data-stu-id="3eab2-111">Open the item</span></span>
- <span data-ttu-id="3eab2-112">Dosya -> Özellikleri -> Internet Başlıkları</span><span class="sxs-lookup"><span data-stu-id="3eab2-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="3eab2-113">veya</span><span class="sxs-lookup"><span data-stu-id="3eab2-113">or</span></span>

<span data-ttu-id="3eab2-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="3eab2-114">**MFCMapi**</span></span>

- <span data-ttu-id="3eab2-115">Gelen kutusundaki öğeye gidin</span><span class="sxs-lookup"><span data-stu-id="3eab2-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="3eab2-116">PR_TRANSPORT_MESSAGE_HEADERS_W arayın</span><span class="sxs-lookup"><span data-stu-id="3eab2-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="3eab2-117">Bu özellikler taşıma ve yönlendirme sırasında belirlenir ve kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="3eab2-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="3eab2-118">Daha fazla sorun giderme için, SPF, DKIM ve.veya DMARC'taki hatalar hakkında Transport Support ile izlemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="3eab2-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>