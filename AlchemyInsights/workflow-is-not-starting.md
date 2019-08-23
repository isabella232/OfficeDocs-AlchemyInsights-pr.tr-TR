---
title: İş akışı başlatılıyor.
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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558009"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="34287-102">İş akışı başlatılıyor.</span><span class="sxs-lookup"><span data-stu-id="34287-102">Workflow is not starting</span></span>

- <span data-ttu-id="34287-103">İş akışları SharePoint 2010 ve SharePoint 2013 başlangıç değil.</span><span class="sxs-lookup"><span data-stu-id="34287-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="34287-104">İş akışınızı başlatılamıyorsa, bir geçici olarak hizmet sorunu olabilir nerede kullanıcıların iş akışı ilerleme ile aralıklı gecikmeler yaşayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="34287-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="34287-105">[Hizmet durumu Panosu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) kuruluşunuzun etkileniyor mu görmek için denetleyin.</span><span class="sxs-lookup"><span data-stu-id="34287-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="34287-106">Bu sorun ilk gördüğünüz bu yana 24 saatten fazla başarılı olması halinde, Lütfen bir destek bileti oturum.</span><span class="sxs-lookup"><span data-stu-id="34287-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="34287-107">Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="34287-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="34287-108">Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="34287-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="34287-109">SharePoint 2010 iş akışı Başlat'ertelendi.</span><span class="sxs-lookup"><span data-stu-id="34287-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="34287-110">Bu, büyük toplu olarak iş akışı tetikleniyorsa oluşur.</span><span class="sxs-lookup"><span data-stu-id="34287-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="34287-111">(örneğin, ne zaman çeşitli öğeler aynı anda eklenir).</span><span class="sxs-lookup"><span data-stu-id="34287-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="34287-112">İş akışları tasarımdan davranış bir gecikme olacak şekilde gerçek zamanlı, çalıştırmak için tasarlanmamış.</span><span class="sxs-lookup"><span data-stu-id="34287-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="34287-113">İş akışı karmaşık Genişletilebilir nesne biçimlendirme dili (XMOL) ise, derleme yavaş olabilir.</span><span class="sxs-lookup"><span data-stu-id="34287-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="34287-114">[Bu](https://support.microsoft.com/en-us/kb/3043697) makalede denetleyin.</span><span class="sxs-lookup"><span data-stu-id="34287-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="34287-115">İş akışını kolaylaştırmak veya Microsoft SharePoint 2013 iş akışı platform türünü kullanarak yeniden tasarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="34287-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="34287-116">İş akışı geçmişini büyüdüyse öğeleri Temizle veya yeni bir geçmiş listesi oluşturmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="34287-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="34287-117">Daha fazla bilgi: [İş Akışı Geçmişi Temizle](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="34287-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="34287-118">İlgili konular</span><span class="sxs-lookup"><span data-stu-id="34287-118">Related topics</span></span>
<span data-ttu-id="34287-119">SharePoint çevrimiçi Microsoft Flow denemek istiyor?</span><span class="sxs-lookup"><span data-stu-id="34287-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="34287-120">Akış oluşturma</span><span class="sxs-lookup"><span data-stu-id="34287-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="34287-121">SharePoint ve akış</span><span class="sxs-lookup"><span data-stu-id="34287-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


