---
title: İş akışı başlat değil
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403763"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="e859e-102">İş akışı başlat değil</span><span class="sxs-lookup"><span data-stu-id="e859e-102">Workflow is not starting</span></span>

- <span data-ttu-id="e859e-103">SharePoint 2010 ve SharePoint 2013 iş akışları başlat değil.</span><span class="sxs-lookup"><span data-stu-id="e859e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="e859e-104">İş akışınız başlatılmışsa, kullanıcıların iş akışı ilerleme durumuyla ilgili aralıklı olarak gecikmeler yaşamaları geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="e859e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="e859e-105">Hizmet Durumu [Panosuna bakarak,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) kurumdan etkilenenin olup olduğunu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="e859e-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="e859e-106">Bu sorunu ilk kez gördükten sonra 24 saati geçtiyse lütfen destek bileti kaydı yapın.</span><span class="sxs-lookup"><span data-stu-id="e859e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e859e-107">Birçok durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="e859e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e859e-108">Lütfen bize çözümü tamamlamak için en az 24 saat süre ver.</span><span class="sxs-lookup"><span data-stu-id="e859e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="e859e-109">SharePoint 2010 iş akışları gecikmeli olarak başlar.</span><span class="sxs-lookup"><span data-stu-id="e859e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="e859e-110">İş akışı büyük toplu işlemlerde tetiklenirse bu durum ortaya çıkar.</span><span class="sxs-lookup"><span data-stu-id="e859e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="e859e-111">(örneğin, aynı anda birkaç öğe ekleniyorsa).</span><span class="sxs-lookup"><span data-stu-id="e859e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="e859e-112">İş akışları gerçek zamanlı olarak çalıştıracak şekilde tasarlanmamalıdır, bu nedenle gecikme tasarım davranışıdır.</span><span class="sxs-lookup"><span data-stu-id="e859e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="e859e-113">İş Akışı Genişletilebilir Nesne İşaretleme Dili (XLANDı) karmaşıksa, derleme işlemi yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="e859e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="e859e-114">Bu [makaleye](https://support.microsoft.com//kb/3043697) bakın.</span><span class="sxs-lookup"><span data-stu-id="e859e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="e859e-115">İş akışını basitleştirmeli veya Microsoft SharePoint 2013 İş Akışı platform türünü kullanarak yeniden tasarlamalı.</span><span class="sxs-lookup"><span data-stu-id="e859e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="e859e-116">İş akışı geçmişiniz büyüdüyse, öğeleri temizlemek veya yeni bir geçmiş listesi oluşturmak iyi olabilir.</span><span class="sxs-lookup"><span data-stu-id="e859e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="e859e-117">Daha Fazla Bilgi : [İş Akışı Geçmişini Temizleme](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="e859e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="e859e-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="e859e-118">Related topics</span></span>
<span data-ttu-id="e859e-119">SharePoint Online'da Microsoft Flow'u denemek mi istiyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="e859e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e859e-120">Akış Oluşturma</span><span class="sxs-lookup"><span data-stu-id="e859e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e859e-121">SharePoint ve Flow</span><span class="sxs-lookup"><span data-stu-id="e859e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
