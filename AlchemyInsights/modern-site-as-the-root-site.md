---
title: Modern site kök site olarak
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232735"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="62992-102">Modern site kök site olarak</span><span class="sxs-lookup"><span data-stu-id="62992-102">Modern site as root site</span></span>

<span data-ttu-id="62992-103">Biz ürün için Klasik site kök sitenizin modern bir site ile takas etmek izin veren yeni bir özellik başlamıştır.</span><span class="sxs-lookup"><span data-stu-id="62992-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="62992-104">[Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) konumunu başka bir siteye sahip bir site, özgün site Arşivlerken takas etmek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="62992-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="62992-105">Ekip sitesi (bir gruba bağlı değil) hem de iletişim Site için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="62992-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="62992-106">Modern bir iletişim sitesi oluşturmak için Klasik kök site silmeyin.</span><span class="sxs-lookup"><span data-stu-id="62992-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="62992-107">Bu Microsoft tarafından desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="62992-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="62992-108">Siteyi geri yüklemek veya aynı URL'de yeni bir site oluşturmak kadar kök site silindiğinde tüm SharePoint siteleri, kuruluşunuzdaki tüm kullanıcılar için erişilebilir hale getirir.</span><span class="sxs-lookup"><span data-stu-id="62992-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="62992-109">Biz bu özellik ileti merkezi aracılığıyla iletişim.</span><span class="sxs-lookup"><span data-stu-id="62992-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="62992-110">Özelliği, Kiracı kısa bir süre sonra açık olması için beklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="62992-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="62992-111">Takas siteleri ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="62992-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="62992-112">Hedef site kısa bir süre için bir "not found" (HTTP 404) hata döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="62992-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="62992-113">İçerik arama dizini güncelleştirmek için recrawled gerekecek.</span><span class="sxs-lookup"><span data-stu-id="62992-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="62992-114">Burada gereken el ile hiçbir adım, bu otomatik olarak yapılacaktır.</span><span class="sxs-lookup"><span data-stu-id="62992-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="62992-115">"Statik" bağlantıları (örneğin, dosya eşitleme ve OneNote dosyaları) bağımlı bir şey elle düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="62992-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="62992-116">Project Server siteleri doğru hala ilişkili olduklarından emin olmak için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="62992-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
