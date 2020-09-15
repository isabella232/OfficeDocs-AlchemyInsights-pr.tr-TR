---
title: SharePoint veya OneDrive 'ı kullanmaya çalışırken bakım iletisi için salt okunur
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670852"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7d33b-102">SharePoint veya OneDrive 'ı kullanmaya çalışırken bakım iletisi için salt okunur</span><span class="sxs-lookup"><span data-stu-id="7d33b-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7d33b-103">Kullanıcılar, aşağıdaki senaryolardan biri için SharePoint veya OneDrive 'ı kullanmaya çalışırken **yalnızca bir salt okunur** ileti alabilir.</span><span class="sxs-lookup"><span data-stu-id="7d33b-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="7d33b-104">Planlanmış veya etkin bir bakım etkinliği.</span><span class="sxs-lookup"><span data-stu-id="7d33b-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="7d33b-105">[Ileti merkezine](https://portal.office.com/adminportal/home#/messagecenter)giderek bunları denetleyin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="7d33b-106">Yüksek öncelikli, etkin bir hizmet olayı olabilir.</span><span class="sxs-lookup"><span data-stu-id="7d33b-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="7d33b-107">[Hizmet durumu](https://portal.office.com/adminportal/home#/servicehealth)'na giderek Danışma belgelerini/olaylarını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="7d33b-108">Sunucularda en çok 30 dak veya bu nedenle en son olabilecek beklenmeyen etkinlikler nedeniyle oluşabilecek küçük bir otomatik düzeltme Kurtarma senaryosu.</span><span class="sxs-lookup"><span data-stu-id="7d33b-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="7d33b-109">Bu küçük kurtarmalar için Ileti merkezi veya hizmet durumu gönderileri yok, ancak yine de normal çok yakında geri dönebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d33b-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="7d33b-110">Çok az, yukarıda listelenen üç senaryodan birinin neden olduğunu ve hizmet geri yüklendiğini gözlemlüyoruz, ancak kullanıcılar tarayıcı önbelleği temizlenmemiştir.</span><span class="sxs-lookup"><span data-stu-id="7d33b-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="7d33b-111">Lütfen siteye gitmeden önce tarayıcı önbelleğini temizlemeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7d33b-112">Microsoft Edge tarayıcınızda **Ayarlar**'ı seçin ve **Gizlilik ve güvenlik**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7d33b-113">**Gezinmeyi temizle**altında, **neyin temizlensin 'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7d33b-114">**Tanımlama bilgileri ve kaydedilmiş Web sitesi verilerini**seçip **Temizle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="7d33b-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7d33b-115">Bu adımlar Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken farklılık gösterebilir.</span><span class="sxs-lookup"><span data-stu-id="7d33b-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7d33b-116">Başka bir seçenek de SharePoint sitenizi veya OneDrive 'ı yeni bir InPrivate penceresinde açar.</span><span class="sxs-lookup"><span data-stu-id="7d33b-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>