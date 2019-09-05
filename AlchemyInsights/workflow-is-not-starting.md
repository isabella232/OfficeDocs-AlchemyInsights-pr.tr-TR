---
title: İş akışı başlatmıyor
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738109"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="937bb-102">İş akışı başlatmıyor</span><span class="sxs-lookup"><span data-stu-id="937bb-102">Workflow is not starting</span></span>

- <span data-ttu-id="937bb-103">SharePoint 2010 ve SharePoint 2013 iş akışları başlatılmıyor.</span><span class="sxs-lookup"><span data-stu-id="937bb-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="937bb-104">İş akışınız başlatılamazsa, kullanıcıların iş akışı ilerlemesinde aralıklı gecikmelerle karşılaşabilecekleri geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="937bb-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="937bb-105">Kuruluşunuzun etkilenip etkilenmeip etkilenmeyin iã§in [Hizmet SaÄ lÄ±k Panosu'](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) nu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="937bb-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="937bb-106">Bu sorunu ilk gördüğünüzden bu yana 24 saatten fazla zaman geçtiyse, lütfen bir destek bileti ni kaydedin.</span><span class="sxs-lookup"><span data-stu-id="937bb-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="937bb-107">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="937bb-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="937bb-108">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="937bb-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="937bb-109">SharePoint 2010 iş akışları başlangıçta gecikti.</span><span class="sxs-lookup"><span data-stu-id="937bb-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="937bb-110">Bu, iş akışı büyük gruplar halinde tetiklenirse oluşur.</span><span class="sxs-lookup"><span data-stu-id="937bb-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="937bb-111">(örneğin, aynı anda birden fazla öğe eklendiğinde).</span><span class="sxs-lookup"><span data-stu-id="937bb-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="937bb-112">İş akışları gerçek zamanlı çalışacak şekilde tasarlanmaz, bu nedenle gecikme tasarım davranışıdır.</span><span class="sxs-lookup"><span data-stu-id="937bb-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="937bb-113">İş Akışı karmaşık genişletilebilir Nesne Biçimlendirme Dili (XMOL) ise, derleme yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="937bb-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="937bb-114">[Bu](https://support.microsoft.com//kb/3043697) makaleyi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="937bb-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="937bb-115">Microsoft SharePoint 2013 İş Akışı platformu türünü kullanarak iş akışını basitleştirmeli veya yeniden tasarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="937bb-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="937bb-116">İş akışı geçmişiniz büyüdüyse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="937bb-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="937bb-117">Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="937bb-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="937bb-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="937bb-118">Related topics</span></span>
<span data-ttu-id="937bb-119">SharePoint Online'da Microsoft Flow'u denemek ister misiniz?</span><span class="sxs-lookup"><span data-stu-id="937bb-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="937bb-120">Akış Oluştur</span><span class="sxs-lookup"><span data-stu-id="937bb-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="937bb-121">SharePoint ve Akış</span><span class="sxs-lookup"><span data-stu-id="937bb-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


