---
title: E-postadan Etkinliklerle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834859"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="957cc-102">E-postadan Etkinliklerle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="957cc-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="957cc-103">Posta kutusu için özelliğin etkinleştirildiğinden emin olun: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="957cc-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="957cc-104">Ardından "E-postadan Etkinlikler" günlüklerine **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="957cc-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="957cc-105">'E-postadan Etkinlikler' günlüklerinde, posta kutusunda öğeyle eşleşen InternetMessageId'i bulun.</span><span class="sxs-lookup"><span data-stu-id="957cc-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="957cc-106">TrustScore, öğenin ekli olup olmadığını belirler.</span><span class="sxs-lookup"><span data-stu-id="957cc-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="957cc-107">Olaylar yalnızca TrustScore = "Trusted" ise eklenir.</span><span class="sxs-lookup"><span data-stu-id="957cc-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="957cc-108">TrustScore, İleti Üst Bilgisinde bulunan SPF, Dkim veya Dmarc özellikleri tarafından belirlenir.</span><span class="sxs-lookup"><span data-stu-id="957cc-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="957cc-109">Bu özellikleri görüntülemek için:</span><span class="sxs-lookup"><span data-stu-id="957cc-109">To view these properties:</span></span>

<span data-ttu-id="957cc-110">**Masaüstü Outlook**</span><span class="sxs-lookup"><span data-stu-id="957cc-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="957cc-111">Öğeyi açma</span><span class="sxs-lookup"><span data-stu-id="957cc-111">Open the item</span></span>
- <span data-ttu-id="957cc-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="957cc-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="957cc-113">veya</span><span class="sxs-lookup"><span data-stu-id="957cc-113">or</span></span>

<span data-ttu-id="957cc-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="957cc-114">**MFCMapi**</span></span>

- <span data-ttu-id="957cc-115">Gelen kutusunda öğeye gider</span><span class="sxs-lookup"><span data-stu-id="957cc-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="957cc-116">Daha fazla PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="957cc-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="957cc-117">Bu özellikler aktarım ve yönlendirme sırasında belirlenir ve kaydedilir.</span><span class="sxs-lookup"><span data-stu-id="957cc-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="957cc-118">Sorun gidermeye yönelik daha fazla sorun gidermek için SPF, DKIM ve.veya DMARC'daki başarısızlıklar hakkında Aktarım Desteği'ne ihtiyacınız olabilir.</span><span class="sxs-lookup"><span data-stu-id="957cc-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>