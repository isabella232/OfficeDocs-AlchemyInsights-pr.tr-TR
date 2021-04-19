---
title: 'AIP: Üstbilgiler ve altbilgiler beklendiği gibi görüntülenmiyor'
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
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821719"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="fdbb6-102">AIP: Üstbilgiler ve altbilgiler beklendiği gibi görüntülenmiyor</span><span class="sxs-lookup"><span data-stu-id="fdbb6-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="fdbb6-103">Görsel işaretlerin beklendiği gibi görüntülenmesiyle ilgili sorunlar yaşıyorsanız, aşağıdaki yönergeleri izleyin:</span><span class="sxs-lookup"><span data-stu-id="fdbb6-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="fdbb6-104">Görsel işaretler uygulandığında [incelemeyi gözden geçirmeyi sağlar.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="fdbb6-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="fdbb6-105">Office etiketlemesi için, [Office 365 içerik işaretleme ve şifrelemesi uygulamanın ne zaman uygulandığını gözden geçirebilirsiniz.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)</span><span class="sxs-lookup"><span data-stu-id="fdbb6-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="fdbb6-106">Var olan üst bilgileri/alt bilgileri kaldırmak için, Diğer etiket çözümlerinden üst bilgileri [ve alt bilgileri kaldırma'ya bakın.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)</span><span class="sxs-lookup"><span data-stu-id="fdbb6-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="fdbb6-107">Sorun hala yaşıyorsanız, Azure Information Protection istemci günlüklerini toplayın ve dışarı aktarıldı günlükleri bu bilete iliştirin.</span><span class="sxs-lookup"><span data-stu-id="fdbb6-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="fdbb6-108">**Azure Information Protection günlüklerini dışarı aktarma**</span><span class="sxs-lookup"><span data-stu-id="fdbb6-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="fdbb6-109">Bir Office belgesi açın veya Outlook'ta yeni e-posta oluşturun.</span><span class="sxs-lookup"><span data-stu-id="fdbb6-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="fdbb6-110">**Koru/Duyarlılık Yardımı ve geri**  >  **bildirim'e tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="fdbb6-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="fdbb6-111">Günlükleri Dışarı **Aktar 'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="fdbb6-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="fdbb6-112">Günlükleri tercih konumunuzla kaydedin ve bunları bu hizmet isteğine iliştirin.</span><span class="sxs-lookup"><span data-stu-id="fdbb6-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="fdbb6-113">Ek bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="fdbb6-113">For additional information, see:</span></span>

- [<span data-ttu-id="fdbb6-114">Azure Information Protection'da görsel işaretlere uygun etiketi yapılandırma</span><span class="sxs-lookup"><span data-stu-id="fdbb6-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="fdbb6-115">Azure Information Protection belgelerini gözden geçirme</span><span class="sxs-lookup"><span data-stu-id="fdbb6-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="fdbb6-116">Azure Information Protection gereksinimleri</span><span class="sxs-lookup"><span data-stu-id="fdbb6-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="fdbb6-117">Azure Information Protection hızlı başlangıç öğreticisi</span><span class="sxs-lookup"><span data-stu-id="fdbb6-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="fdbb6-118">Azure Information Protection istemcisini indirin</span><span class="sxs-lookup"><span data-stu-id="fdbb6-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
