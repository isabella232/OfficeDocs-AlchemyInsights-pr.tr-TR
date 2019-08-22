---
title: Klasik kök sitenizin Modern bir site ile takas
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501099"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="4709a-102">Klasik kök sitenizin Modern bir site ile takas</span><span class="sxs-lookup"><span data-stu-id="4709a-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="4709a-103">Ortamınızı önce Nisan 2019 ayarlarsanız, modern bir siteye kök sitenizin Microsoft PowerShell kullanarak değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="4709a-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="4709a-104">Sitenizin kök kullanmak istediğiniz farklı bir site varsa, (takas) kök site ile değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4709a-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="4709a-105">[Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) konumunu başka bir siteye sahip bir site, özgün site Arşivlerken takas etmek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="4709a-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="4709a-106">Ekip sitesi (bir gruba bağlı değil) hem de iletişim Site için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="4709a-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="4709a-107">Ek yetenekler kullanılmaya başlanan yakında olanak tanıyacak şekilde sitesindeki içeriği kullanarak tutmak, ancak varolan sitenin iletişim siteye dönüştürmek.</span><span class="sxs-lookup"><span data-stu-id="4709a-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="4709a-108">Bu yetenekleri yavaş yavaş piyasaya çıkacağı.</span><span class="sxs-lookup"><span data-stu-id="4709a-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="4709a-109">Güncelleştirmeler için Office 365 ileti merkezi bakmaya devam edin.</span><span class="sxs-lookup"><span data-stu-id="4709a-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="4709a-110">Takas siteleri ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="4709a-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="4709a-111">Hedef site kısa bir süre için bir "not found" (HTTP 404) hata döndürebilir.</span><span class="sxs-lookup"><span data-stu-id="4709a-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="4709a-112">İçerik arama dizini güncelleştirmek için recrawled gerekecek.</span><span class="sxs-lookup"><span data-stu-id="4709a-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="4709a-113">Gereken el ile hiçbir adım - bu otomatik olarak yapılacaktır.</span><span class="sxs-lookup"><span data-stu-id="4709a-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="4709a-114">"Statik" bağlantıları (örneğin, dosya eşitleme ve OneNote dosyaları) bağımlı bir şey elle düzeltilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="4709a-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="4709a-115">Kaynak site kuruluş haber sitesi varsa, URL'yi güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="4709a-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="4709a-116">Tüm kuruluş haber sitelerin bir listesini alın.</span><span class="sxs-lookup"><span data-stu-id="4709a-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="4709a-117">Project Server siteleri doğru hala ilişkili olduklarından emin olmak için doğrulanması gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="4709a-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





