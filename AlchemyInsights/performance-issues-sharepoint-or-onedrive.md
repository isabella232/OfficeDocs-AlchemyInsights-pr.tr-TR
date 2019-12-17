---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068441"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4e77a-102">SharePoint veya OneDrive birden çok kullanıcı için yavaş, erişilemez veya kullanılamıyor</span><span class="sxs-lookup"><span data-stu-id="4e77a-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="4e77a-103">SharePoint veya OneDrive yavaş, erişilemez veya kullanılamayabilir veya hizmet in kullanılamayan veya 503 hata görüntüleyebilir:</span><span class="sxs-lookup"><span data-stu-id="4e77a-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="4e77a-104">SharePoint veya OneDrive siteniz birden çok kullanıcı için yavaş sayılsa veya gecikirse, kullanıcıların SharePoint sitelerine veya OneDrive içeriğine erişirken aralıklı gecikmeler veya gezinme hataları yla karşılaştığı geçici bir hizmet sorunu olabilir.</span><span class="sxs-lookup"><span data-stu-id="4e77a-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="4e77a-105">Kuruluşunuzun etkilenip etkilenmeip etkilenmeyin iã§in [Hizmet sistem durumu panosunu](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="4e77a-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="4e77a-106">Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken *bir 503 sunucu meşgul* hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="4e77a-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="4e77a-107">Bu hata, SharePoint hizmeti içinde daraltma neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="4e77a-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4e77a-108">SharePoint Online, SharePoint Online hizmetinin en iyi performansını ve güvenilirliğini korumak için azaltma yı kullanır.</span><span class="sxs-lookup"><span data-stu-id="4e77a-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4e77a-109">Azaltma, kaynakların aşırı kullanımını önlemek için kullanıcı eylemlerinin veya eşzamanlı çağrıların (komut dosyası veya koda göre) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="4e77a-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="4e77a-110">Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="4e77a-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="4e77a-111">**Klasik** veya **modern** bir SharePoint sitesi veya sayfasıyla yavaş performans yaşıyorsanız, sayfaları analiz etmek için [Sayfa Tanılama aracını](https://aka.ms/perftool) kullanarak.</span><span class="sxs-lookup"><span data-stu-id="4e77a-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="4e77a-112">Genel yavaş performans yaşamaya devam ediyorsanız, lütfen bu makalenin altındaki kaynakları gözden geçirin: [SharePoint Online için performans atonuna giriş](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="4e77a-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  