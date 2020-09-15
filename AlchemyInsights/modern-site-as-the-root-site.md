---
title: Kök site olarak modern site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666890"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="56955-102">Kök site olarak modern site</span><span class="sxs-lookup"><span data-stu-id="56955-102">Modern site as root site</span></span>

<span data-ttu-id="56955-103">[Klasik site kök sitenizi modern bir siteyle takas](https://docs.microsoft.com/sharepoint/modern-root-site)etme olanağı tanıyan yeni bir özellik piyasaya çıkarılacak.</span><span class="sxs-lookup"><span data-stu-id="56955-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="56955-104">Özgün siteyi arşivlerken, bir sitenin konumunu başka bir siteyle değiştirmek için [çağır-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 'ı kullanın.</span><span class="sxs-lookup"><span data-stu-id="56955-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="56955-105">Hem ekip sitesi (gruba bağlı değil) hem de Iletişim sitesi için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="56955-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="56955-106">Modern bir Iletişim sitesi oluşturmak için klasik kök sitenizi silmeyin.</span><span class="sxs-lookup"><span data-stu-id="56955-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="56955-107">Bu, Microsoft tarafından desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="56955-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="56955-108">Kök site silindiğinde, siz siteyi geri yükleyinceye veya aynı URL 'de yeni bir site oluşturana kadar kuruluşunuzdaki tüm SharePoint sitelerinin tüm kullanıcılara erişilemez olmasını sağlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="56955-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="56955-109">Bu özelliğe ileti merkezi aracılığıyla iletişim kuracağız.</span><span class="sxs-lookup"><span data-stu-id="56955-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="56955-110">Bu özelliğin kiracınızda hemen açık olmasını beklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="56955-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="56955-111">Siteleri değiştirme ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="56955-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="56955-112">Hedef site kısa bir süre boyunca "bulunamadı" (HTTP 404) hatası döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="56955-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="56955-113">İçerik, arama dizinini güncelleştirmek için yeniden gezilecek.</span><span class="sxs-lookup"><span data-stu-id="56955-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="56955-114">Burada el ile adım gerekmeyecektir, bu işlem otomatik olarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="56955-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="56955-115">"Statik" bağlantılara (dosya eşitleme ve OneNote dosyaları gibi) bağlı olarak, el ile düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="56955-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="56955-116">Project Server sitelerinin doğru ilişkilendirilmeleri için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="56955-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
