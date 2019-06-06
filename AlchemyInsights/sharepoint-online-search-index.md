---
title: SharePoint çevrimiçi arama sözlüklerde yönetme
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736072"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="7a7b4-102">Çevrimiçi arama SharePoint içinde</span><span class="sxs-lookup"><span data-stu-id="7a7b4-102">Search in SharePoint Online</span></span>

<span data-ttu-id="7a7b4-103">İçeriği gezinme ve kullanıcıların ne onlar için SharePoint çevrimiçi aradığınız bulmak arama dizini eklenir.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="7a7b4-104">İçeriği otomatik olarak tabanlı (gezinme zamanlaması değiştirilemez) önceden tanımlanmış gezinme zamanlaması üzerinde gezildiğinde.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="7a7b4-105">Gezgin en son gezinmeden sonra değişti ve dizini güncelleştirir içeriğini seçer.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="7a7b4-106">İçerik gezilen ve dizinin güncelleştirildiğinden emin olmak için aşağıdaki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="7a7b4-107">Site içeriğini aranabilir hale getirerek içerik bulunabilir olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="7a7b4-108">Daha fazla bilgi için bkz: [aranabilir olmasını sitesindeki içeriği etkinleştirme](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="7a7b4-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="7a7b4-109">Arama dizinine yaptığınız değişiklikler yansıtılır önce yönetilen bir özellik değiştiğinde ya da gezinme ve yönetilen Eşleme değişti site özelliklerini yeniden gezilen olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="7a7b4-110">Site arama şemada yapılan değişiklikleri ve otomatik olarak değil gerçek sitesi Gezgin olur çünkü yeniden dizin oluşturur.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="7a7b4-111">Daha fazla bilgi için bkz: [el ile istek gezinme ve bir kitaplık veya listenin bir site dizini yeniden oluşturuluyor](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="7a7b4-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="7a7b4-112">El ile bir gezinme ve hala bir sorunla karşılaştığınız varsa görmek için tam yeniden dizin isteyen sonra en az 24 saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="7a7b4-113">Gezinme ve tam dizin yeniden başlattığından beri 24 saatten fazla geçmişse, Lütfen destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="7a7b4-114">Çoğu durumda, biz zaten bir çözüm üzerinde çalışıyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7a7b4-115">Lütfen bize bir çözüm tamamlamak için en az 24 saat verin.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="7a7b4-116">**Önemli**: bir site, belge (kitaplık) veya bir liste silinir ve hala gösterir arama sonuçlarında ise, kullanıcılar bir hata 404 Dosya bulunamadı erişilmeye çalışılırken almalısınız.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="7a7b4-117">Bu sorun bir destek çalışması için daha fazla araştırma olarak oturum açmış olmanız.</span><span class="sxs-lookup"><span data-stu-id="7a7b4-117">This issue should be logged as a support case for further investigation.</span></span> 



