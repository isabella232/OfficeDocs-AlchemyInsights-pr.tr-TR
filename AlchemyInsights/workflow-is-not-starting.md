---
title: İş akışı başlatmıyor
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049357"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b4f28-102">İş akışı başlatmıyor</span><span class="sxs-lookup"><span data-stu-id="b4f28-102">Workflow is not starting</span></span>

- <span data-ttu-id="b4f28-103">SharePoint 2010 ve SharePoint 2013 iş akışları başlatılmıyor.</span><span class="sxs-lookup"><span data-stu-id="b4f28-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b4f28-104">İş akışınız başlatılamazsa, kullanıcıların iş akışı ilerlemesinde aralıklı gecikmelerle karşılaşabilecekleri geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="b4f28-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b4f28-105">Kuruluşunuzun etkilenip etkilenmeip etkilenmeyin iã§in [Hizmet SaÄ lÄ±k Panosu'](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) nu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="b4f28-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b4f28-106">Bu sorunu ilk gördüğünüzden bu yana 24 saatten fazla zaman geçtiyse, lütfen bir destek bileti ni kaydedin.</span><span class="sxs-lookup"><span data-stu-id="b4f28-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b4f28-107">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="b4f28-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b4f28-108">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="b4f28-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b4f28-109">SharePoint 2010 iş akışları başlangıçta gecikti.</span><span class="sxs-lookup"><span data-stu-id="b4f28-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b4f28-110">Bu, iş akışı büyük gruplar halinde tetiklenirse oluşur.</span><span class="sxs-lookup"><span data-stu-id="b4f28-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b4f28-111">(örneğin, aynı anda birden fazla öğe eklendiğinde).</span><span class="sxs-lookup"><span data-stu-id="b4f28-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b4f28-112">İş akışları gerçek zamanlı çalışacak şekilde tasarlanmaz, bu nedenle gecikme tasarım davranışıdır.</span><span class="sxs-lookup"><span data-stu-id="b4f28-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b4f28-113">İş Akışı karmaşık genişletilebilir Nesne Biçimlendirme Dili (XMOL) ise, derleme yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="b4f28-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b4f28-114">Bu makaleyi kontrol [edin.](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="b4f28-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b4f28-115">Microsoft SharePoint 2013 İş Akışı platformu türünü kullanarak iş akışını basitleştirmeli veya yeniden tasarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b4f28-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b4f28-116">İş akışı geçmişiniz büyüdüyse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b4f28-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b4f28-117">Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b4f28-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b4f28-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="b4f28-118">Related topics</span></span>
<span data-ttu-id="b4f28-119">SharePoint Online'da Microsoft Flow'u denemek ister misiniz?</span><span class="sxs-lookup"><span data-stu-id="b4f28-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b4f28-120">Akış Oluştur</span><span class="sxs-lookup"><span data-stu-id="b4f28-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b4f28-121">SharePoint ve Akış</span><span class="sxs-lookup"><span data-stu-id="b4f28-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


