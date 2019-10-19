---
title: Klasik kök sitenizi Modern bir siteyle değiştirin
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749280"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="8b499-102">Klasik kök sitenizi Modern bir siteyle değiştirin</span><span class="sxs-lookup"><span data-stu-id="8b499-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="8b499-103">Ortamınız Nisan 2019'dan önce ayarlanmışsa, Microsoft PowerShell'i kullanarak kök sitenizi modern bir siteyle değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8b499-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="8b499-104">Kök siteniz olarak kullanmak istediğiniz farklı bir siteniz varsa, kök siteyi onunla değiştirebilir [(değiştirebilirsiniz).](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="8b499-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="8b499-105">Orijinal siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın.</span><span class="sxs-lookup"><span data-stu-id="8b499-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="8b499-106">Hem Takım Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="8b499-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="8b499-107">Sitedeki içeriği kullanmaya devam etmenizi, ancak varolan siteyi bir iletişim sitesine dönüştürmenizi sağlayacak ek özellikler yakında sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="8b499-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="8b499-108">Bu yetenekler kademeli olarak kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="8b499-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="8b499-109">Güncelleştirmeler için Office 365 İleti Merkezi'ni denetlemeye devam edin.</span><span class="sxs-lookup"><span data-stu-id="8b499-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="8b499-110">Siteleri değiştirme yle ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="8b499-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="8b499-111">Hedef site kısa bir süre için bir "bulunamadı" (HTTP 404) hatası döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="8b499-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="8b499-112">Arama dizinini güncelleştirmek için içeriğin yeniden taranması gerekir.</span><span class="sxs-lookup"><span data-stu-id="8b499-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="8b499-113">El ile adım gerekmez - bu otomatik olarak yapılacaktır.</span><span class="sxs-lookup"><span data-stu-id="8b499-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="8b499-114">"Statik" bağlantılara (Dosya Eşitlemi ve OneNote dosyaları gibi) bağlı olan her şeyin el ile düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="8b499-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="8b499-115">Kaynak site bir kuruluş haber sitesiyse, URL'yi güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="8b499-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="8b499-116">Tüm organizasyonel haber sitelerinin listesini alın.</span><span class="sxs-lookup"><span data-stu-id="8b499-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="8b499-117">Project Server sitelerinin hala doğru ilişkili olduğundan emin olmak için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="8b499-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





