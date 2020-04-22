---
title: dosya adı ile aynı en iyisidir
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676553"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="18cc9-102">Gerekli Simya Başlık H1, H2's çalışmıyor.</span><span class="sxs-lookup"><span data-stu-id="18cc9-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="18cc9-103">Simya yazarlık için en iyi uygulamalar ve yönergeler:</span><span class="sxs-lookup"><span data-stu-id="18cc9-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="18cc9-104">**Alchemy Insights'ı klasörlere yerleştirmeyin**- bu url yapısını bozar.</span><span class="sxs-lookup"><span data-stu-id="18cc9-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="18cc9-105">Bunu düzeltmeye çalışıyoruz.</span><span class="sxs-lookup"><span data-stu-id="18cc9-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="18cc9-106">**AlchemyInsights** klasöründeki dosyalarda, boşluklar için tireli küçük dosya adları olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="18cc9-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="18cc9-107">***nasıl etkinleştirmek-dava-tutun***.</span><span class="sxs-lookup"><span data-stu-id="18cc9-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="18cc9-108">Ms.custom alanına [Simya Ortağı portalından](https://alchemyportal.azurewebsites.net) Kural Kimliği veya kova kimliği ekleyin.</span><span class="sxs-lookup"><span data-stu-id="18cc9-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="18cc9-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="18cc9-109">ex.</span></span> <span data-ttu-id="18cc9-110">***ms.özel: 100021***</span><span class="sxs-lookup"><span data-stu-id="18cc9-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="18cc9-111">Şablonolarak bu dosyanın üst kısmındaki meta verilerin geri kalanını kullanın.</span><span class="sxs-lookup"><span data-stu-id="18cc9-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="18cc9-112">[Simya İş Ortağı portalında,](https://alchemyportal.azurewebsites.net)Müşteri Öngörü başlığı bölümüne **gidin:** ve bunu bilgi edinmek için H1 başlığınız için bir başlangıç noktası olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="18cc9-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="18cc9-113">Simya Insights üst kısmında sadece tek bir H1 olmalı ya da üretim de kıracak.</span><span class="sxs-lookup"><span data-stu-id="18cc9-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="18cc9-114">H2'ler, ayrı bölümleri belirtmek için **kalın** veya diğer kuralları kullanmaz.</span><span class="sxs-lookup"><span data-stu-id="18cc9-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="18cc9-115">Ardından, Simya Kuralı sayfasının Müşteri Öngörüleri bölümündeki taslak materyali kullanarak gövde metnini doldurun</span><span class="sxs-lookup"><span data-stu-id="18cc9-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="18cc9-116">Madde işaretli listeler iyi</span><span class="sxs-lookup"><span data-stu-id="18cc9-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="18cc9-117">Numaralanmış listeler de</span><span class="sxs-lookup"><span data-stu-id="18cc9-117">Numbered lists too</span></span>
    1. <span data-ttu-id="18cc9-118">**Kalın** ve *italik* a-ok vardır</span><span class="sxs-lookup"><span data-stu-id="18cc9-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="18cc9-119">Bağlantılar her zaman ya **"web bağlantıları" / dış** VEYA **UI öğeleri ne**derin bağlantılar değil, iç bağlantılar olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="18cc9-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="18cc9-120">Resimler şu anda resmi olarak desteklenmez, ancak yol haritasında yer almaktadır.</span><span class="sxs-lookup"><span data-stu-id="18cc9-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="18cc9-121">Ve bu gerçekten biraz fazla uzun.</span><span class="sxs-lookup"><span data-stu-id="18cc9-121">And this is really already a bit too long.</span></span> <span data-ttu-id="18cc9-122">En iyi uygulama yaklaşık 400 karakter ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="18cc9-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="18cc9-123">İçeriğiniz hazır olduğunda, canlı şubeye çekin.</span><span class="sxs-lookup"><span data-stu-id="18cc9-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="18cc9-124">Ardından [Simya Ortağı portalına](https://alchemyportal.azurewebsites.net) gidin ve dosya adını url alanına girin.</span><span class="sxs-lookup"><span data-stu-id="18cc9-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 