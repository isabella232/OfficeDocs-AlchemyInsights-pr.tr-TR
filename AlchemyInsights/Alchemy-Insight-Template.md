---
title: dosyaadı ile aynı
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664154"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="09c08-102">"Gerekli Alchemy üstbilgisi H1, H2's çalışmıyor."</span><span class="sxs-lookup"><span data-stu-id="09c08-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="09c08-103">Alchemy yazma için en iyi yöntemler ve yönergeler:</span><span class="sxs-lookup"><span data-stu-id="09c08-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="09c08-104">**Klasörlerde iç Içe Alchemy öngörülerini**vermeyin-bu, URL yapısını bozar.</span><span class="sxs-lookup"><span data-stu-id="09c08-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="09c08-105">Bu.</span><span class="sxs-lookup"><span data-stu-id="09c08-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="09c08-106">**Alchemyya** klasöründeki dosyalar, boşluklar EX için kısa çizgiler içeren küçük dosya adlarına sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="09c08-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="09c08-107">***nasıl yapılır-özelliğini etkinleştirme***.</span><span class="sxs-lookup"><span data-stu-id="09c08-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="09c08-108">MS. özel alanına [Alchemy Iş ortağı portalından](https://alchemyportal.azurewebsites.net) kural kimliğini veya demet kimliğini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="09c08-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="09c08-109">NEX.</span><span class="sxs-lookup"><span data-stu-id="09c08-109">ex.</span></span> <span data-ttu-id="09c08-110">***MS. özel: 100021***</span><span class="sxs-lookup"><span data-stu-id="09c08-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="09c08-111">Bu dosyanın en üstündeki meta verilerin kalan kısmını şablonunuzu kullanın.</span><span class="sxs-lookup"><span data-stu-id="09c08-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="09c08-112">[Alchemy Iş ortağı portalında](https://alchemyportal.azurewebsites.net), **Müşteri Insight başlığı** bölümüne gidin: ve bu konuyu, bu anlayış için H1 başlığının başlangıç noktası olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="09c08-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="09c08-113">Alchemy Insights 'ın en üstte yalnızca tek bir H1 OLMALıDıR veya üretime bölünmez.</span><span class="sxs-lookup"><span data-stu-id="09c08-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="09c08-114">H2s işleme yoksa ayrı bölümleri belirtmek için **kalın** veya başka bir kural kullanın.</span><span class="sxs-lookup"><span data-stu-id="09c08-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="09c08-115">Ardından, Alchemy kuralı sayfasının müşteri Öngörüler bölümündeki taslak malzemesini kullanarak gövde metnini doldurun</span><span class="sxs-lookup"><span data-stu-id="09c08-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="09c08-116">Madde işaretli listeler iyidir</span><span class="sxs-lookup"><span data-stu-id="09c08-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="09c08-117">Numaralandırılmış listeler çok</span><span class="sxs-lookup"><span data-stu-id="09c08-117">Numbered lists too</span></span>
    1. <span data-ttu-id="09c08-118">**Kalın** ve *italik*</span><span class="sxs-lookup"><span data-stu-id="09c08-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="09c08-119">Bağlantılar, iç bağlantılar değil, **Kullanıcı Arabirimi öğelerine** **"Web 'e bağlantılar"/dış** veya derin bağlantılarına sahip olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="09c08-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="09c08-120">Resimler Şu anda bir şekilde desteklenmez, ancak yol haritası.</span><span class="sxs-lookup"><span data-stu-id="09c08-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="09c08-121">Bu, gerçekten çok uzun.</span><span class="sxs-lookup"><span data-stu-id="09c08-121">And this is really already a bit too long.</span></span> <span data-ttu-id="09c08-122">En iyi uygulama 400 karakter---------------------------------</span><span class="sxs-lookup"><span data-stu-id="09c08-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="09c08-123">İçeriğiniz hazır olduğunda, bunu canlı şubeye çekin.</span><span class="sxs-lookup"><span data-stu-id="09c08-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="09c08-124">Ardından [Alchemy Iş ortağı portalına](https://alchemyportal.azurewebsites.net) gidin ve URL alanına dosya adını girin.</span><span class="sxs-lookup"><span data-stu-id="09c08-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 