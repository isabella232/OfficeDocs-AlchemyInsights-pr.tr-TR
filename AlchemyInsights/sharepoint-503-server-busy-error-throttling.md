---
title: SharePoint çevrimiçi azaltma
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761278"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="bf5a2-102">SharePoint çevrimiçi azaltma</span><span class="sxs-lookup"><span data-stu-id="bf5a2-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="bf5a2-103">Kullanıcılar bir 503 alabilirsiniz sunucu SharePoint veya OneDrive sitelerine gitmek çalışırken meşgul hata olur.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="bf5a2-104">SharePoint hizmet içinde bastırarak bu hataya neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="bf5a2-105">SharePoint çevrimiçi azaltma en iyi performans ve güvenilirlik SharePoint çevrimiçi hizmet korumak için kullanır.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="bf5a2-106">Sınırları azaltmayı veya eşzamanlı kullanıcı eylemlerinin sayısı kaynakların aşırı kullanımı önlemek için (komut dosyası veya kod) çağırır.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="bf5a2-107">Daraltılmış, özel kod nedeniyle olduğu zaman % 99.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="bf5a2-108">Bakın, [bastırma veya SharePoint çevrimiçi engellenmiş kaçının](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)azaltma hakkında daha fazla bilgi için.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="bf5a2-109">Bu hata azaltma için ilgisiz olduğunu düşünüyorsanız, [İleti Merkezi](https://portal.office.com/adminportal/home#/MessageCenter)giderek, Kiracı üzerinde gerçekleşen etkin bakım olup olmadığını denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="bf5a2-110">Son olarak, tüm danışma /, oluşabilecek KAZALARI için denetlemek için [Hizmet durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret edin emin olun.</span><span class="sxs-lookup"><span data-stu-id="bf5a2-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

