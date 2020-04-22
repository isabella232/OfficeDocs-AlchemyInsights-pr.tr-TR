---
title: İçerik SharePoint arama sonuçlarında görünmüyor
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705681"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="40265-102">İçerik SharePoint arama sonuçlarında görünmüyor</span><span class="sxs-lookup"><span data-stu-id="40265-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="40265-103">Beklenen içerik arama sonuçlarında görünmüyorsa aşağıdaki sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="40265-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="40265-104">Beklenen içeriği içeren **sitenin,** içeriğin arama sonuçlarında görünmesine izin verecek şekilde ayarlı olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="40265-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="40265-105">[Arama sonuçlarında bir sitedeki içeriği göster'deki](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="40265-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="40265-106">Beklenen içeriği içeren **listenin** veya **kitaplığın,** içeriğin arama sonuçlarında görünmesine izin verecek şekilde ayarlı olup olmadığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="40265-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="40265-107">[Arama sonuçlarında listelerden veya kitaplıklardan içeriği göster'deki](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="40265-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="40265-108">Sayfanın, belgenin veya özel sayfa düzeninin Ana sürüm olarak yayımlandığını **doğrulayın.**</span><span class="sxs-lookup"><span data-stu-id="40265-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="40265-109">[Arama'da](https://go.microsoft.com/fwlink/?linkid=874525)3.</span><span class="sxs-lookup"><span data-stu-id="40265-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="40265-110">Kullanıcının içeriği görüntüleme **izinlerine** sahip olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="40265-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="40265-111">[SharePoint'te izin düzeylerini anlama](https://docs.microsoft.com/sharepoint/understanding-permission-levels)adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="40265-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="40265-112">Arama şeması yeni yönetilen bir özellik ekleyerek, yönetilen bir özelliği düzenleyerek veya yönetilen bir özelliği kaldırarak değiştirildiyse, tarama ve yeniden dizin istemek gerekir.</span><span class="sxs-lookup"><span data-stu-id="40265-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="40265-113">Bir [sitenin, kitaplığın veya listenin el ile tarama ve yeniden dizini oluşturmasını manuel olarak isteyerek](https://docs.microsoft.com/sharepoint/crawl-site-content)içeriği **yeniden dizine ekleyin.**</span><span class="sxs-lookup"><span data-stu-id="40265-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="40265-114">Bu işlem biraz zaman alabilir, sonuçları tekrar kontrol etmeden önce 24 saat bekleyebilir.</span><span class="sxs-lookup"><span data-stu-id="40265-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="40265-115">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="40265-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
