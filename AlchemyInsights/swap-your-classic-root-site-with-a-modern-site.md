---
title: Klasik kök sitenizi modern bir siteyle değiştirme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691199"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="665aa-102">Klasik kök sitenizi modern bir siteyle değiştirme</span><span class="sxs-lookup"><span data-stu-id="665aa-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="665aa-103">Ortamınız 2019 Nisan 'dan önce ayarlanmışsa, Microsoft PowerShell kullanarak kök sitenizi modern bir siteye dönüştürebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="665aa-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="665aa-104">Kök siteniz olarak kullanmak istediğiniz farklı bir siteniz varsa, [kök siteyi onunla değiştirebilirsiniz (takas edebilirsiniz)](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="665aa-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="665aa-105">Özgün siteyi arşivlerken, bir sitenin konumunu başka bir siteyle değiştirmek için [çağır-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 'ı kullanın.</span><span class="sxs-lookup"><span data-stu-id="665aa-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="665aa-106">Hem ekip sitesi (gruba bağlı değil) hem de Iletişim sitesi için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="665aa-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="665aa-107">Sitedeki içeriği kullanmaya devam edecek ancak var olan siteyi bir iletişim sitesine dönüştürebilecek olan ek özellikler yakında kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="665aa-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="665aa-108">Bu özellikler aşamalı olarak kullanıma sunulacaktır.</span><span class="sxs-lookup"><span data-stu-id="665aa-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="665aa-109">Güncelleştirmelerin Ileti merkezini denetlemeye devam edin.</span><span class="sxs-lookup"><span data-stu-id="665aa-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="665aa-110">Siteleri değiştirme ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="665aa-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="665aa-111">Hedef site kısa bir süre boyunca "bulunamadı" (HTTP 404) hatası döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="665aa-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="665aa-112">İçerik, arama dizinini güncelleştirmek için yeniden gezilecek.</span><span class="sxs-lookup"><span data-stu-id="665aa-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="665aa-113">El ile adım gerekmez; Bu işlem otomatik olarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="665aa-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="665aa-114">"Statik" bağlantılara (dosya eşitleme ve OneNote dosyaları gibi) bağlı olarak, el ile düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="665aa-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="665aa-115">Kaynak site bir kuruluş haber sitesidir, URL 'YI güncelleyin.</span><span class="sxs-lookup"><span data-stu-id="665aa-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="665aa-116">Tüm kuruluş haberleri sitelerinin listesini alın.</span><span class="sxs-lookup"><span data-stu-id="665aa-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="665aa-117">Project Server sitelerinin doğru ilişkilendirilmeleri için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="665aa-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
