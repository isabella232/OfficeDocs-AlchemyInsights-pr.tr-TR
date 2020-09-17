---
title: İş akışı başlamıyor
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794787"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="21c40-102">İş akışı başlamıyor</span><span class="sxs-lookup"><span data-stu-id="21c40-102">Workflow is not starting</span></span>

- <span data-ttu-id="21c40-103">SharePoint 2010 ve SharePoint 2013 iş akışları başlamıyor.</span><span class="sxs-lookup"><span data-stu-id="21c40-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="21c40-104">İş akışınız başlatılamıyorsa, kullanıcıların iş akışı ilerlemesiyle aralıklı gecikmelere neden olabileceği geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="21c40-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="21c40-105">Kuruluşunuzun [etkilenmediklerini görmek Için hizmet durumu panosunu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="21c40-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="21c40-106">Bu sorunu ilk kez gördüğünüzde 24 saatten uzun bir süreyi geçmişse, lütfen bir destek bileti günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="21c40-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="21c40-107">Birçok durumda bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="21c40-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="21c40-108">Lütfen çözümü tamamlamak için en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="21c40-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="21c40-109">SharePoint 2010 iş akışları başlangıçta gecikti.</span><span class="sxs-lookup"><span data-stu-id="21c40-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="21c40-110">Bu, iş akışı büyük toplu işlerle tetiklendiğinde gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="21c40-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="21c40-111">(örneğin, bir kerede birkaç öğe eklendiğinde).</span><span class="sxs-lookup"><span data-stu-id="21c40-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="21c40-112">İş akışları gerçek zamanlı çalışacak şekilde tasarlanmamıştır, böylece bir gecikme tasarım davranışıdır.</span><span class="sxs-lookup"><span data-stu-id="21c40-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="21c40-113">Iş akışı karmaşık genişletilebilir nesne Işaretleme dili (XMOL) ise, derleme yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="21c40-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="21c40-114">[Bu](https://support.microsoft.com//kb/3043697) makaleyi denetleyin.</span><span class="sxs-lookup"><span data-stu-id="21c40-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="21c40-115">Microsoft SharePoint 2013 Iş akışı Platform türünü kullanarak iş akışını basitleştirin veya yeniden tasarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="21c40-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="21c40-116">İş akışı geçmişiniz büyürse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="21c40-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="21c40-117">Daha fazla bilgi: [Iş akışı geçmişini temizle](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="21c40-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="21c40-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="21c40-118">Related topics</span></span>
<span data-ttu-id="21c40-119">SharePoint Online 'da Microsoft akışını denemek mi istiyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="21c40-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="21c40-120">Akış oluştur</span><span class="sxs-lookup"><span data-stu-id="21c40-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="21c40-121">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="21c40-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


