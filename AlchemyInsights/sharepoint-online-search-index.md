---
title: Çevrimiçi arama SharePoint içinde
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059272"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="8b712-102">Çevrimiçi arama SharePoint içinde</span><span class="sxs-lookup"><span data-stu-id="8b712-102">Search in SharePoint Online</span></span>

<span data-ttu-id="8b712-103">İçeriği gezinme ve kullanıcıların ne onlar için SharePoint çevrimiçi aradığınız bulmak arama dizini eklenir.</span><span class="sxs-lookup"><span data-stu-id="8b712-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="8b712-104">İçeriği otomatik olarak tabanlı (gezinme zamanlaması değiştirilemez) önceden tanımlanmış gezinme zamanlaması üzerinde gezildiğinde.</span><span class="sxs-lookup"><span data-stu-id="8b712-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="8b712-105">Gezgin en son gezinmeden sonra değişti ve dizini güncelleştirir içeriğini seçer.</span><span class="sxs-lookup"><span data-stu-id="8b712-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="8b712-106">İçerik gezilen ve dizinin güncelleştirildiğinden emin olmak için aşağıdakilere dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="8b712-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="8b712-107">[Site içeriğini aranabilir hale](https://docs.microsoft.com/sharepoint/make-site-content-searchable)getirerek içerik bulunabilir olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8b712-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="8b712-108">Arama dizinine yaptığınız değişiklikler yansıtılır önce yönetilen bir özellik değiştiğinde ya da gezinme ve yönetilen Eşleme değişti site özelliklerini yeniden gezilen olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="8b712-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="8b712-109">Site arama şemada yapılan değişiklikleri ve otomatik olarak değil gerçek sitesi Gezgin olur çünkü yeniden dizin oluşturur.</span><span class="sxs-lookup"><span data-stu-id="8b712-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="8b712-110">Daha fazla bilgi için bkz: [el ile istek gezinme ve bir kitaplık veya listenin bir site dizini yeniden oluşturuluyor](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="8b712-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="8b712-111">El ile bir gezinme ve hala bir sorunla karşılaştığınız varsa görmek için tam yeniden dizin isteyen sonra en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="8b712-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="8b712-112">Gezinme ve tam dizin yeniden başlattığından beri 24 saatten fazla geçmişse, Lütfen destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="8b712-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="8b712-113">Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="8b712-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8b712-114">Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="8b712-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Önemli!]<span data-ttu-id="8b712-115">: bir site, belge (kitaplık) veya bir liste silinir ve hala gösterir arama sonuçlarında ise, kullanıcılar bir **Hata 404 Dosya bulunamadı** erişmek çalışırken almalısınız.</span><span class="sxs-lookup"><span data-stu-id="8b712-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="8b712-116">Bu sorun bir destek çalışması için daha fazla araştırma olarak oturum açmış olmanız.</span><span class="sxs-lookup"><span data-stu-id="8b712-116">This issue should be logged as a support case for further investigation.</span></span> 



