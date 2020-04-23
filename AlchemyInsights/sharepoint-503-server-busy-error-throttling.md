---
title: SharePoint Online Azaltma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742229"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="29351-102">SharePoint Online Azaltma</span><span class="sxs-lookup"><span data-stu-id="29351-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="29351-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="29351-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="29351-104">**503 sunucu meşgul hata**</span><span class="sxs-lookup"><span data-stu-id="29351-104">**503 server is busy error**</span></span>

<span data-ttu-id="29351-105">Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken bir 503 sunucu meşgul hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="29351-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="29351-106">Bu hata, SharePoint hizmeti içinde daraltma neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="29351-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="29351-107">SharePoint Online, SharePoint Online hizmetinin en iyi düzeyde performans ve güvenilirliğini sürdürmesi için kısıtlama kullanıyor.</span><span class="sxs-lookup"><span data-stu-id="29351-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="29351-108">Kısıtlama işlemi, kaynakların aşırı kullanımını önlemek için kullanıcı eylemi veya eşzamanlı çağrı (betik veya kod ile) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="29351-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="29351-109">Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="29351-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="29351-110">Bu hatanın azaltmayla ilgisi olmadığını düşünüyorsanız, [İleti merkezi'ne](https://portal.office.com/adminportal/home#/MessageCenter)yönlendirerek kiracınızda etkin bir bakım olup olmadığını kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29351-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="29351-111">Son olarak, oluşabilecek danışma/olayları kontrol etmek için [Hizmet Durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="29351-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

