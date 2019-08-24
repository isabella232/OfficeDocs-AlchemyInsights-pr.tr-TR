---
title: SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620743"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="219a6-102">SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur</span><span class="sxs-lookup"><span data-stu-id="219a6-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="219a6-103">Kullanıcılar, SharePoint veya OneDrive aşağıdaki senaryolardan birini kullanmaya çalışırken bir **Bakım için salt okunur** ileti alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="219a6-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="219a6-104">Bir etkin veya planlı bakım etkinlikleri.</span><span class="sxs-lookup"><span data-stu-id="219a6-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="219a6-105">Onlar için [İleti Merkezi](https://portal.office.com/adminportal/home#/messagecenter)giderek denetleyin.</span><span class="sxs-lookup"><span data-stu-id="219a6-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="219a6-106">Oluşabilecek yüksek öncelikli etkin servis olayı.</span><span class="sxs-lookup"><span data-stu-id="219a6-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="219a6-107">[Sağlık Hizmeti](https://portal.office.com/adminportal/home#/servicehealth)için giderek herhangi danışma/olayları denetleyin.</span><span class="sxs-lookup"><span data-stu-id="219a6-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="219a6-108">Beklenmeyen olaylar nedeniyle 30 min ya da bunu daha az için son sunucularda olmuyor, küçük otomatik düzeltme kurtarma senaryosu.</span><span class="sxs-lookup"><span data-stu-id="219a6-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="219a6-109">Hiçbir ileti merkezi vardır veya Sağlık Hizmeti bu küçük kurtarmaları için deftere naklettiği ancak normal olarak çok yakında olmalı.</span><span class="sxs-lookup"><span data-stu-id="219a6-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="219a6-110">Çok az sayıda olayda yukarıda listelenen üç senaryolardan birini neden olmuştur ve hizmet geri yüklendi ancak kullanıcıların tarayıcı önbellek temizlenmiş taşınmadığından Kutlandı.</span><span class="sxs-lookup"><span data-stu-id="219a6-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="219a6-111">Lütfen siteye gitmeden önce tarayıcı önbelleği temizlemek deneyin.</span><span class="sxs-lookup"><span data-stu-id="219a6-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="219a6-112">Microsoft Edge tarayıcınızın **ayarlarını**seçin ve ardından **Gizlilik ve güvenlik**seçin.</span><span class="sxs-lookup"><span data-stu-id="219a6-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="219a6-113">**Clear göz**altında **temizlemek ne seçin**seçin.</span><span class="sxs-lookup"><span data-stu-id="219a6-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="219a6-114">**Tanımlama bilgileri ve kaydedilmiş Web sitesi verilerini**seçin ve **Temizle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="219a6-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="219a6-115">Bu adımlar, Mozilla Firefox veya Google Chrome gibi başka tarayıcıları kullanırken, farklı olabilir.</span><span class="sxs-lookup"><span data-stu-id="219a6-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="219a6-116">SharePoint sitesi veya OneDrive yeni InPrivate penceresinde açmak için başka bir seçenek olacaktır.</span><span class="sxs-lookup"><span data-stu-id="219a6-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>