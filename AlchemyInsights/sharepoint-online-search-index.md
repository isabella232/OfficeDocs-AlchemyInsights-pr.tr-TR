---
title: SharePoint Online'da Ara
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044063"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="cb494-102">SharePoint Online'da içerik tarama ve dizine eklenme</span><span class="sxs-lookup"><span data-stu-id="cb494-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="cb494-103">Kullanıcıların SharePoint Online'da aradıklarını bulmaları için içerik taranmalı ve arama dizinine eklenmelidir.</span><span class="sxs-lookup"><span data-stu-id="cb494-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="cb494-104">İçerik önceden tanımlanmış bir tarama zamanlamasına göre otomatik olarak türünilir (tarama zamanlaması değiştirilemez).</span><span class="sxs-lookup"><span data-stu-id="cb494-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="cb494-105">Tarayıcı, son gezinmeden bu yana değişen içeriği alır ve dizini güncelleştirir.</span><span class="sxs-lookup"><span data-stu-id="cb494-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="cb494-106">İçeriğin tarandığından ve dizinin güncelleştirdiğinden emin olmak için aşağıdakileri unutmayın:</span><span class="sxs-lookup"><span data-stu-id="cb494-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="cb494-107">[Site içeriğini aranabilir hale getirerek](https://docs.microsoft.com/sharepoint/make-site-content-searchable)içeriğin bulunabilmesini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="cb494-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="cb494-108">Yönetilen bir özelliği değiştirdiğinizde veya taranmış ve yönetilen özelliklerin eşlemeyi değiştirdiğinizde, değişikliklerinizin arama dizinine yansıtılmadan önce sitenin yeniden taranması gerekir.</span><span class="sxs-lookup"><span data-stu-id="cb494-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="cb494-109">Değişiklikleriniz gerçek sitede değil, arama şemasında yapıldığından, tarayıcı siteyi otomatik olarak yeniden dizine yapmaz.</span><span class="sxs-lookup"><span data-stu-id="cb494-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="cb494-110">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/sharepoint/crawl-site-conten)</span><span class="sxs-lookup"><span data-stu-id="cb494-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="cb494-111">Bir sorun yaşamaya devam edip olmadığınızı görmek için el ile tarama ve tam yeniden dizini istedikten sonra en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="cb494-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="cb494-112">Tarama ve tam yeniden dizini başlatmanız üzerinden 24 saatten fazla zaman geçtiyse, lütfen bir destek örneğini günlüğe kaydedin.</span><span class="sxs-lookup"><span data-stu-id="cb494-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="cb494-113">Çoğu durumda, zaten bir çözüm üzerinde çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="cb494-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cb494-114">Lütfen bir çözümü tamamlamamız için bize en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="cb494-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cb494-115">Bir site, belge (kitaplık) veya bir liste silinmişse ve arama sonuçlarında hala gösteriliyorsa, kullanıcılar siteye erişmeye çalışırken Bulunamadı bir **Hata 404 Dosyası** almalıdır.</span><span class="sxs-lookup"><span data-stu-id="cb494-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="cb494-116">Bu sorun, daha fazla araştırma için bir destek durumu olarak günlüğe kaydedilmelidir.</span><span class="sxs-lookup"><span data-stu-id="cb494-116">This issue should be logged as a support case for further investigation.</span></span> 



