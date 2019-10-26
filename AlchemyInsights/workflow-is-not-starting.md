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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738109"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="16d2e-102">İş akışı başlatmıyor</span><span class="sxs-lookup"><span data-stu-id="16d2e-102">Workflow is not starting</span></span>

- <span data-ttu-id="16d2e-103">SharePoint 2010 ve SharePoint 2013 iş akışları başlatılmıyor.</span><span class="sxs-lookup"><span data-stu-id="16d2e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="16d2e-104">İş akışınız başlatılamazsa, kullanıcıların iş akışı ilerlemesinde aralıklı gecikmelerle karşılaşabilecekleri geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="16d2e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="16d2e-105">Kuruluşunuzun etkilenip etkilenmeip etkilenmeyin iã§in [Hizmet SaÄ lÄ±k Panosu'](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) nu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="16d2e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="16d2e-106">Bu sorunu ilk gördüğünüzden bu yana 24 saatten fazla zaman geçtiyse, lütfen bir destek bileti ni kaydedin.</span><span class="sxs-lookup"><span data-stu-id="16d2e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="16d2e-107">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="16d2e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="16d2e-108">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="16d2e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="16d2e-109">SharePoint 2010 iş akışları başlangıçta gecikti.</span><span class="sxs-lookup"><span data-stu-id="16d2e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="16d2e-110">Bu, iş akışı büyük gruplar halinde tetiklenirse oluşur.</span><span class="sxs-lookup"><span data-stu-id="16d2e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="16d2e-111">(örneğin, aynı anda birden fazla öğe eklendiğinde).</span><span class="sxs-lookup"><span data-stu-id="16d2e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="16d2e-112">İş akışları gerçek zamanlı çalışacak şekilde tasarlanmaz, bu nedenle gecikme tasarım davranışıdır.</span><span class="sxs-lookup"><span data-stu-id="16d2e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="16d2e-113">İş Akışı karmaşık genişletilebilir Nesne Biçimlendirme Dili (XMOL) ise, derleme yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="16d2e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="16d2e-114">Bu makaleyi kontrol [edin.](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="16d2e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="16d2e-115">Microsoft SharePoint 2013 İş Akışı platformu türünü kullanarak iş akışını basitleştirmeli veya yeniden tasarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="16d2e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="16d2e-116">İş akışı geçmişiniz büyüdüyse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="16d2e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="16d2e-117">Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="16d2e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="16d2e-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="16d2e-118">Related topics</span></span>
<span data-ttu-id="16d2e-119">SharePoint Online'da Microsoft Flow'u denemek ister misiniz?</span><span class="sxs-lookup"><span data-stu-id="16d2e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="16d2e-120">Akış Oluştur</span><span class="sxs-lookup"><span data-stu-id="16d2e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="16d2e-121">SharePoint ve Akış</span><span class="sxs-lookup"><span data-stu-id="16d2e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


