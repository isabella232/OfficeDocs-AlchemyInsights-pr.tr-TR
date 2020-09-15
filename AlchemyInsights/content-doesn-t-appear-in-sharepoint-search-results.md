---
title: SharePoint arama sonuçlarında içerik görünmüyor
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713150"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="69f26-102">SharePoint arama sonuçlarında içerik görünmüyor</span><span class="sxs-lookup"><span data-stu-id="69f26-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="69f26-103">Beklenen içeriğin arama sonuçlarında görüntülenmediği durumlarda bu sorun giderme adımlarını izleyin:</span><span class="sxs-lookup"><span data-stu-id="69f26-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="69f26-104">Beklenen içeriği içeren **sitenin** , arama sonuçlarında içeriğin görüntülenmesine izin verecek şekilde ayarlandığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="69f26-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="69f26-105">[Arama sonuçlarında bir sitedeki Içeriği gösterme](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)konusundaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="69f26-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="69f26-106">Beklenen içeriği içeren **liste** veya **kitaplığın** , içerik arama sonuçlarında görünmesine izin verecek şekilde ayarlandığını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="69f26-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="69f26-107">[Arama sonuçlarında listelerden veya kitaplıklardaki Içeriği gösterme](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)konusundaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="69f26-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="69f26-108">Sayfa, belge veya özel sayfa düzeninin **ana sürüm** olarak yayımlandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="69f26-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="69f26-109">Arama sırasında 3. adıma kadar, [SharePoint Online 'daki tüm sonuçları döndürmez](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="69f26-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="69f26-110">Kullanıcının içeriği görüntüleme **izni** olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="69f26-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="69f26-111">[SharePoint 'teki izin düzeylerini anlama](https://docs.microsoft.com/sharepoint/understanding-permission-levels)konusundaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="69f26-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="69f26-112">Arama şeması yeni yönetilen bir özellik ekleyerek, yönetilen bir özelliği düzenleyerek veya yönetilen bir özelliği kaldırarak bir gezinme isteğinde bulunulduktan sonra gezinmeyi ve yeniden indeki gerekli olacak şekilde değiştirdiyseniz.</span><span class="sxs-lookup"><span data-stu-id="69f26-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="69f26-113">Bir [sitenin, kitaplığın veya listenin el ile gezinmeyi ve yeniden dizinini oluşturma](https://docs.microsoft.com/sharepoint/crawl-site-content)konusundaki adımları Izleyerek içeriği **yeniden dizin haline** koyun.</span><span class="sxs-lookup"><span data-stu-id="69f26-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="69f26-114">Bu biraz zaman alabilir, sonuçları yeniden gözden geçirmeden önce 24 saat beklemeniz gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="69f26-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="69f26-115">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="69f26-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
