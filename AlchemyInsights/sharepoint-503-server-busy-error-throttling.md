---
title: SharePoint Online azaltma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773867"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="56ae3-102">SharePoint Online azaltma</span><span class="sxs-lookup"><span data-stu-id="56ae3-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="56ae3-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="56ae3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="56ae3-104">**503 sunucusu meşgul**</span><span class="sxs-lookup"><span data-stu-id="56ae3-104">**503 server is busy error**</span></span>

<span data-ttu-id="56ae3-105">Kullanıcılar, SharePoint veya OneDrive sitelerine gitmeye çalışırken bir 503 sunucusu alabilir.</span><span class="sxs-lookup"><span data-stu-id="56ae3-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="56ae3-106">Bu hata, SharePoint hizmeti içinde azaltma nedeniyle oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="56ae3-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="56ae3-107">SharePoint Online, SharePoint Online hizmetinin en iyi düzeyde performans ve güvenilirliğini sürdürmesi için kısıtlama kullanıyor.</span><span class="sxs-lookup"><span data-stu-id="56ae3-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="56ae3-108">Kısıtlama işlemi, kaynakların aşırı kullanımını önlemek için kullanıcı eylemi veya eşzamanlı çağrı (betik veya kod ile) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="56ae3-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="56ae3-109">Azaltma ile ilgili daha fazla bilgi için, [SharePoint Online 'da azaltma veya engellenmekten kaçının](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="56ae3-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="56ae3-110">Bu hatanın azaltma konusunda ilgisiz olduğunu düşünüyorsanız, [ileti merkezine](https://portal.office.com/adminportal/home#/MessageCenter)giderek kiracınızda etkin bakım olup olmadığını denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="56ae3-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="56ae3-111">Son olarak, oluşabilecek Danışma belgelerini/olaylarını denetlemek için [hizmet durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="56ae3-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

