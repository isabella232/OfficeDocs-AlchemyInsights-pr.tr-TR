---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771921"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="6d900-102">SharePoint veya OneDrive yavaş, erişilemez veya birden çok kullanıcı için kullanılamaz</span><span class="sxs-lookup"><span data-stu-id="6d900-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="6d900-103">SharePoint veya OneDrive yavaş, erişilemez veya kullanılamıyor olabilir ya da bazı nedenlerden dolayı hizmet kullanılamıyor veya 503 hataları görüntülenebilir:</span><span class="sxs-lookup"><span data-stu-id="6d900-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="6d900-104">SharePoint veya OneDrive siteniz yavaş veya birden çok kullanıcı için gecikirse, SharePoint sitelerine veya OneDrive içeriğine erişirken kullanıcıların aralıklı gecikmelere veya gezinti hatalarıyla karşılaştikleri geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="6d900-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="6d900-105">Kuruluşunuzun [etkilenmediklerini görmek Için hizmet durumu panosunu](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="6d900-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="6d900-106">Kullanıcılar, SharePoint veya OneDrive sitelerine gitmeye çalışırken bir *503 sunucusu* alabilir.</span><span class="sxs-lookup"><span data-stu-id="6d900-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="6d900-107">Bu hata, SharePoint hizmeti içinde azaltma nedeniyle oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="6d900-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6d900-108">SharePoint Online, SharePoint Online hizmetinin en iyi düzeyde performans ve güvenilirliğini sürdürmesi için kısıtlama kullanıyor.</span><span class="sxs-lookup"><span data-stu-id="6d900-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6d900-109">Kısıtlama işlemi, kaynakların aşırı kullanımını önlemek için kullanıcı eylemi veya eşzamanlı çağrı (betik veya kod ile) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="6d900-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6d900-110">Azaltma ile ilgili daha fazla bilgi için, [SharePoint Online 'da azaltma veya engellenmekten kaçının](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6d900-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="6d900-111">**Klasik** veya **modern** bir SharePoint sitesi veya sayfasıyla yavaş performansla karşılaşırsanız, sayfaları çözümlemek için [sayfa tanı aracını](https://aka.ms/perftool) kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6d900-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="6d900-112">Genel yavaş performansla karşılaşmaya devam ediyorsanız, lütfen bu makalenin altındaki kaynakları inceleyin: [SharePoint Online için performans ayarlamaya giriş](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="6d900-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  