---
title: 'aynı dosya adı iyi olduğu gibi [kural #-açıklama]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634524"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="2f460-102">Gerekli Alchemy başlık H1, H2's çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="2f460-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="2f460-103">En iyi yöntemleri ve yönergeleri Alchemy yazmak için:</span><span class="sxs-lookup"><span data-stu-id="2f460-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="2f460-104">**Klasörlerde Alchemy görüşleri geçirmeyin**- Bu url yapısı kesecektir.</span><span class="sxs-lookup"><span data-stu-id="2f460-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="2f460-105">Biz bu düzeltme içine bakıyorsunuzdur.</span><span class="sxs-lookup"><span data-stu-id="2f460-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="2f460-106">**AlchemyInsights** klasöründeki dosyaları, dosya adını kural kimliği ve [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) kural adı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="2f460-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="2f460-107">ex.</span><span class="sxs-lookup"><span data-stu-id="2f460-107">ex.</span></span> <span data-ttu-id="2f460-108">***976-How-to-Enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="2f460-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="2f460-109">Meta veriler, bu dosyanın en üstünde, şablon olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="2f460-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="2f460-110">Hiçbir şey gereklidir.</span><span class="sxs-lookup"><span data-stu-id="2f460-110">Nothing else is required.</span></span>
1. <span data-ttu-id="2f460-111">[Alchemy ortak portalı](https://alchemyportal.azurewebsites.net)bölümüne gidin **Müşteri Insight Başlık:** ve H1 başlığınızın Insight için işaret eden bir başlangıç olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="2f460-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="2f460-112">Üstünde sahip tek bir H1 görüşleri Alchemy olmalıdır veya üretimde kesintiye uğrar.</span><span class="sxs-lookup"><span data-stu-id="2f460-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="2f460-113">H2s, bunu kullanmak **Kalın** veya ayrı bölümler belirtmek için diğer kuralları işlemek yoktur.</span><span class="sxs-lookup"><span data-stu-id="2f460-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="2f460-114">Ardından, gövde metni Alchemy kural sayfanın müşteri görüşleri bölümünde taslak malzeme kullanarak doldurun</span><span class="sxs-lookup"><span data-stu-id="2f460-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="2f460-115">Madde işaretli listeler ince</span><span class="sxs-lookup"><span data-stu-id="2f460-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="2f460-116">Çok numaralı listeler</span><span class="sxs-lookup"><span data-stu-id="2f460-116">Numbered lists too</span></span>
    1. <span data-ttu-id="2f460-117">**Kalın** ve *İtalik* a-ok</span><span class="sxs-lookup"><span data-stu-id="2f460-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="2f460-118">Bağlantıları her zaman olması gerekir ya da **"Bağlantılar Web" / dış** veya **UI öğelerine derin bağlantılar**, değil iç bağlantılar.</span><span class="sxs-lookup"><span data-stu-id="2f460-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="2f460-119">Ve bu gerçekten zaten biraz fazla uzun.</span><span class="sxs-lookup"><span data-stu-id="2f460-119">And this is really already a bit too long.</span></span> <span data-ttu-id="2f460-120">Yaklaşık 400 karakter en iyi uygulamadır---</span><span class="sxs-lookup"><span data-stu-id="2f460-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="2f460-121">İçeriğinizi hazır olduktan sonra canlı dala çeker.</span><span class="sxs-lookup"><span data-stu-id="2f460-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="2f460-122">Daha sonra [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) gidin ve dosya adı url alanına girin.</span><span class="sxs-lookup"><span data-stu-id="2f460-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="2f460-123">Gözden geçirilmiş ve yayımlanan Insight "Evet" diyor emin olun ve sonra güncelleştirme Kuralı'nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2f460-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="2f460-124">**(Bu prettier yakında serbest portal - yeni sürümünde görünecektir.)** 
 ![url alanı](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="2f460-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

