---
title: Çevrimiçi arama SharePoint içinde
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507651"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="6901c-102">İçeriği gezinme ve SharePoint Çevrimiçi dizinleme</span><span class="sxs-lookup"><span data-stu-id="6901c-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="6901c-103">İçeriği gezinme ve kullanıcıların ne onlar için SharePoint çevrimiçi aradığınız bulmak arama dizini eklenir.</span><span class="sxs-lookup"><span data-stu-id="6901c-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="6901c-104">İçeriği otomatik olarak tabanlı (gezinme zamanlaması değiştirilemez) önceden tanımlanmış gezinme zamanlaması üzerinde gezildiğinde.</span><span class="sxs-lookup"><span data-stu-id="6901c-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="6901c-105">Gezgin en son gezinmeden sonra değişti ve dizini güncelleştirir içeriğini seçer.</span><span class="sxs-lookup"><span data-stu-id="6901c-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="6901c-106">İçerik gezilen ve dizinin güncelleştirildiğinden emin olmak için aşağıdakilere dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="6901c-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="6901c-107">[Site içeriğini aranabilir hale](https://docs.microsoft.com/sharepoint/make-site-content-searchable)getirerek içerik bulunabilir olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="6901c-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="6901c-108">Arama dizinine yaptığınız değişiklikler yansıtılır önce yönetilen bir özellik değiştiğinde ya da gezinme ve yönetilen Eşleme değişti site özelliklerini yeniden gezilen olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6901c-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="6901c-109">Site arama şemada yapılan değişiklikleri ve otomatik olarak değil gerçek sitesi Gezgin olur çünkü yeniden dizin oluşturur.</span><span class="sxs-lookup"><span data-stu-id="6901c-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="6901c-110">Daha fazla bilgi için bkz: [el ile istek gezinme ve bir kitaplık veya listenin bir site dizini yeniden oluşturuluyor](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="6901c-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="6901c-111">El ile bir gezinme ve hala bir sorunla karşılaştığınız varsa görmek için tam yeniden dizin isteyen sonra en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="6901c-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="6901c-112">Gezinme ve tam dizin yeniden başlattığından beri 24 saatten fazla geçmişse, Lütfen destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="6901c-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="6901c-113">Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="6901c-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6901c-114">Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="6901c-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6901c-115">Bir site, belge (kitaplık) veya bir liste silindi ve görüntülenmeye devam eder arama sonuçlarında kullanıcıların bir **Hata 404 Dosya bulunamadı** erişmek çalışırken almalısınız.</span><span class="sxs-lookup"><span data-stu-id="6901c-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="6901c-116">Bu sorun bir destek çalışması için daha fazla araştırma olarak oturum açmış olmanız.</span><span class="sxs-lookup"><span data-stu-id="6901c-116">This issue should be logged as a support case for further investigation.</span></span> 



