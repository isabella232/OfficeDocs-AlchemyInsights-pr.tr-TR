---
title: Kök site olarak modern site
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753924"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="caded-102">Kök site olarak modern site</span><span class="sxs-lookup"><span data-stu-id="caded-102">Modern site as root site</span></span>

<span data-ttu-id="caded-103">Biz modern bir site ile klasik site [kök sitesi takas](https://docs.microsoft.com/sharepoint/modern-root-site)sağlayacak yeni bir özellik piyasaya başladı.</span><span class="sxs-lookup"><span data-stu-id="caded-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="caded-104">Orijinal siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın.</span><span class="sxs-lookup"><span data-stu-id="caded-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="caded-105">Hem Takım Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="caded-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="caded-106">Modern bir İletişim Sitesi oluşturmak için klasik kök sitenizi silmeyin.</span><span class="sxs-lookup"><span data-stu-id="caded-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="caded-107">Bu Microsoft tarafından desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="caded-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="caded-108">Siteyi geri yükleyene veya aynı URL'de yeni bir site oluşturana kadar, kök siteyi sevebilmek, kuruluşunuzdaki tüm SharePoint sitelerini tüm kullanıcılar tarafından erişilemez hale getirir.</span><span class="sxs-lookup"><span data-stu-id="caded-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="caded-109">Bu özelliği mesaj merkezi aracılığıyla ileteceğiz.</span><span class="sxs-lookup"><span data-stu-id="caded-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="caded-110">Özelliğin kısa süre içinde kiracınızda açık olmasını beklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="caded-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="caded-111">Siteleri değiştirme yle ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="caded-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="caded-112">Hedef site kısa bir süre için bir "bulunamadı" (HTTP 404) hatası döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="caded-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="caded-113">Arama dizinini güncelleştirmek için içeriğin yeniden taranması gerekir.</span><span class="sxs-lookup"><span data-stu-id="caded-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="caded-114">Burada herhangi bir manuel adım gereklidir, bu otomatik olarak yapılacaktır.</span><span class="sxs-lookup"><span data-stu-id="caded-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="caded-115">"Statik" bağlantılara (Dosya Eşitlemi ve OneNote dosyaları gibi) bağlı olan her şeyin el ile düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="caded-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="caded-116">Project Server sitelerinin hala doğru ilişkili olduğundan emin olmak için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="caded-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
