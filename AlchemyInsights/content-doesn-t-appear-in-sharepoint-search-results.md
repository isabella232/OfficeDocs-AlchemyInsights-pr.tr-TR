---
title: İçerik SharePoint arama sonuçlarında görünmüyor
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363845"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="438a8-102">İçerik SharePoint arama sonuçlarında görünmüyor</span><span class="sxs-lookup"><span data-stu-id="438a8-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="438a8-103">Bunlar beklenen içeriği arama sonuçlarında görünmüyor zaman sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="438a8-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="438a8-104">Beklenen içerik içeren **site** içeriği arama sonuçlarında görünmesine izin verecek şekilde ayarlanmış olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="438a8-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="438a8-105">[Arama sonuçlarında bir sitedeki içerik göster](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)' ndaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="438a8-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="438a8-106">**Liste** veya **kitaplık** beklenen içerik içeren içeriği arama sonuçlarında görünmesine izin verecek şekilde ayarlanmış olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="438a8-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="438a8-107">[İçerik listeleri veya kitaplıkları arama sonuçlarında Göster](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)' ndaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="438a8-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="438a8-108">Sayfası, belge veya özel sayfa düzeni olarak yayımlandığını doğrulamak bir **ana sürüm.**</span><span class="sxs-lookup"><span data-stu-id="438a8-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="438a8-109">Adım 3 [Arama SharePoint çevrimiçi tüm sonuçları döndürmüyor](https://go.microsoft.com/fwlink/?linkid=874525)izleyin.</span><span class="sxs-lookup"><span data-stu-id="438a8-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="438a8-110">Kullanıcı içeriğini görüntülemek için **izinlere** sahip olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="438a8-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="438a8-111">[SharePoint izin düzeylerini anlama'ndaki](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="438a8-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="438a8-112">Yeni bir yönetilen özellik ekleyerek arama şeması değiştirilmişse, gezinme ve yeniden dizin oluşturur yönetilen özellik düzenleyerek veya kaldırarak sonra isteyen bir yönetilen özellik gerekli olacaktır.</span><span class="sxs-lookup"><span data-stu-id="438a8-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="438a8-113">**Yeniden dizin** içeriği [el ile istek gezinme ve sitesini, bir kitaplık veya liste dizin yeniden oluşturma](https://docs.microsoft.com/sharepoint/crawl-site-content)adımları izleyerek.</span><span class="sxs-lookup"><span data-stu-id="438a8-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="438a8-114">Bu biraz zaman alır, sonuçları yeniden denetlemeden önce 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="438a8-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="438a8-115">Daha fazla bilgi için bkz: [aranabilir olmasını sitesindeki içeriği etkinleştirme](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="438a8-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
