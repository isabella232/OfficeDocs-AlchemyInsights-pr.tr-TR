---
title: SharePoint Online Azaltma
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048636"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c2f65-102">SharePoint Online Azaltma</span><span class="sxs-lookup"><span data-stu-id="c2f65-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="c2f65-103">Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken bir 503 sunucu meşgul hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="c2f65-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="c2f65-104">Bu hata, SharePoint hizmeti içinde daraltma neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="c2f65-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c2f65-105">SharePoint Online, SharePoint Online hizmetinin en iyi performansını ve güvenilirliğini korumak için azaltma yı kullanır.</span><span class="sxs-lookup"><span data-stu-id="c2f65-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c2f65-106">Azaltma, kaynakların aşırı kullanımını önlemek için kullanıcı eylemlerinin veya eşzamanlı çağrıların (komut dosyası veya koda göre) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="c2f65-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="c2f65-107">Eğer daraltılırsanız, zamanın %99'u özel kod yüzündendir.</span><span class="sxs-lookup"><span data-stu-id="c2f65-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="c2f65-108">Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="c2f65-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="c2f65-109">Bu hatanın azaltmayla ilgisi olmadığını düşünüyorsanız, [İleti merkezi'ne](https://portal.office.com/adminportal/home#/MessageCenter)yönlendirerek kiracınızda etkin bir bakım olup olmadığını kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c2f65-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="c2f65-110">Son olarak, oluşabilecek danışma/olayları kontrol etmek için [Hizmet Durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="c2f65-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

