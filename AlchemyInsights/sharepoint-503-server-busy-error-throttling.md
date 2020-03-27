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
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958755"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="f9e07-102">SharePoint Online Azaltma</span><span class="sxs-lookup"><span data-stu-id="f9e07-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="f9e07-103">**Önemli**: Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin yüksek oranda kullanılabilir kalmasını sağlamak için adımlar atıyoruz – Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Ayarlamaları'nı](https://aka.ms/ODSPAdjustments) ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="f9e07-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f9e07-104">**503 sunucu meşgul hata**</span><span class="sxs-lookup"><span data-stu-id="f9e07-104">**503 server is busy error**</span></span>

<span data-ttu-id="f9e07-105">Kullanıcılar SharePoint veya OneDrive sitelerine gezinmeye çalışırken bir 503 sunucu meşgul hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="f9e07-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="f9e07-106">Bu hata, SharePoint hizmeti içinde daraltma neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="f9e07-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="f9e07-107">SharePoint Online, SharePoint Online hizmetinin en iyi performansını ve güvenilirliğini korumak için azaltma yı kullanır.</span><span class="sxs-lookup"><span data-stu-id="f9e07-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f9e07-108">Azaltma, kaynakların aşırı kullanımını önlemek için kullanıcı eylemlerinin veya eşzamanlı çağrıların (komut dosyası veya koda göre) sayısını sınırlar.</span><span class="sxs-lookup"><span data-stu-id="f9e07-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="f9e07-109">Azaltma hakkında daha fazla bilgi için [SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="f9e07-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="f9e07-110">Bu hatanın azaltmayla ilgisi olmadığını düşünüyorsanız, [İleti merkezi'ne](https://portal.office.com/adminportal/home#/MessageCenter)yönlendirerek kiracınızda etkin bir bakım olup olmadığını kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f9e07-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="f9e07-111">Son olarak, oluşabilecek danışma/olayları kontrol etmek için [Hizmet Durumu](https://portal.office.com/adminportal/home#/servicehealth) sayfasını ziyaret ettiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="f9e07-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

