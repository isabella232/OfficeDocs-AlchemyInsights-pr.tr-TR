---
title: SharePoint veya OneDrive'ı kullanmaya çalışırken Yalnızca Bakım için Okuma iletisi
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051301"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="fb78b-102">SharePoint veya OneDrive'ı kullanmaya çalışırken Yalnızca Bakım için Okuma iletisi</span><span class="sxs-lookup"><span data-stu-id="fb78b-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="fb78b-103">Kullanıcılar, aşağıdaki senaryolardan biri için SharePoint veya OneDrive'ı kullanmaya çalışırken **Yalnızca Bakım için** Salt Okuma iletisi alabilir.</span><span class="sxs-lookup"><span data-stu-id="fb78b-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="fb78b-104">Planlı veya etkin bir bakım faaliyeti.</span><span class="sxs-lookup"><span data-stu-id="fb78b-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="fb78b-105">[İleti Merkezi'ne](https://portal.office.com/adminportal/home#/messagecenter)yönlendirerek bunları kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fb78b-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="fb78b-106">Meydana gelmiş olabilecek yüksek öncelikli, etkin bir hizmet olayı.</span><span class="sxs-lookup"><span data-stu-id="fb78b-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="fb78b-107">[Hizmet Durumu'na](https://portal.office.com/adminportal/home#/servicehealth)yönlendirerek herhangi bir danışma/olay olup olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="fb78b-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="fb78b-108">Sunucularda beklenmeyen olaylar nedeniyle meydana gelebilecek ve 30 dakikadan daha az süregelebilecek küçük bir otomatik iyileşme kurtarma senaryosu.</span><span class="sxs-lookup"><span data-stu-id="fb78b-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="fb78b-109">Bu küçük kurtarmalar için Mesaj Merkezi veya Hizmet Sağlık mesajları vardır ama çok yakında normale geri olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fb78b-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="fb78b-110">Çok az durumda, yukarıda listelenen üç senaryodan birinin neden olduğunu ve hizmetin geri yüklendiğini, ancak kullanıcıların tarayıcı önbelleğinin temizlenmediğini gözlemledik.</span><span class="sxs-lookup"><span data-stu-id="fb78b-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="fb78b-111">Lütfen siteye gitmeden önce tarayıcı önbelleğini temizlemeye çalış.</span><span class="sxs-lookup"><span data-stu-id="fb78b-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="fb78b-112">Microsoft Edge tarayıcınızda **Ayarlar'ı**seçin ve ardından **Gizlilik ve Güvenlik'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="fb78b-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="fb78b-113">**Net tarama**altında, **neyi temizleyeceğini seç'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="fb78b-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="fb78b-114">**Çerezleri ve kaydedilmiş web sitesi verilerini**seçin ve **Temizle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="fb78b-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="fb78b-115">Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken bu adımlar farklı olabilir.</span><span class="sxs-lookup"><span data-stu-id="fb78b-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="fb78b-116">Başka bir seçenek, SharePoint sitenizi veya OneDrive'ınızı yeni bir InPrivate penceresinde açmak olacaktır.</span><span class="sxs-lookup"><span data-stu-id="fb78b-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>