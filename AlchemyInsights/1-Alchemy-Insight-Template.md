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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939331"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="ab4de-102">Gerekli Alchemy başlık H1, H2's çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="ab4de-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="ab4de-103">En iyi yöntemleri ve yönergeleri Alchemy yazmak için:</span><span class="sxs-lookup"><span data-stu-id="ab4de-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="ab4de-p101">**Klasörlerde Alchemy görüşleri geçirmeyin**- Bu url yapısı kesecektir. Biz bu düzeltme içine bakıyorsunuzdur.</span><span class="sxs-lookup"><span data-stu-id="ab4de-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="ab4de-106">**AlchemyInsights** klasöründeki dosyaları, dosya adını kural kimliği ve [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) kural adı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ab4de-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="ab4de-p102">örnek ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="ab4de-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="ab4de-p103">Meta veriler, bu dosyanın en üstünde, şablon olarak kullanın. Hiçbir şey gereklidir.</span><span class="sxs-lookup"><span data-stu-id="ab4de-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="ab4de-111">[Alchemy ortak portalı](https://alchemyportal.azurewebsites.net)bölümüne gidin **Müşteri Insight Başlık:** ve H1 başlığınızın Insight için işaret eden bir başlangıç olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="ab4de-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ab4de-p104">Üstünde sahip tek bir H1 görüşleri Alchemy olmalıdır veya üretimde kesintiye uğrar. H2s, bunu kullanmak **Kalın** veya ayrı bölümler belirtmek için diğer kuralları işlemek yoktur.</span><span class="sxs-lookup"><span data-stu-id="ab4de-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ab4de-114">Ardından, gövde metni Alchemy kural sayfanın müşteri görüşleri bölümünde taslak malzeme kullanarak doldurun</span><span class="sxs-lookup"><span data-stu-id="ab4de-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ab4de-115">Madde işaretli listeler ince</span><span class="sxs-lookup"><span data-stu-id="ab4de-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ab4de-116">Çok numaralı listeler</span><span class="sxs-lookup"><span data-stu-id="ab4de-116">Numbered lists too</span></span>
    1. <span data-ttu-id="ab4de-117">**Kalın** ve *İtalik* a-ok</span><span class="sxs-lookup"><span data-stu-id="ab4de-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ab4de-118">Bağlantıları her zaman olması gerekir ya da **"Bağlantılar Web" / dış** veya **UI öğelerine derin bağlantılar**, değil iç bağlantılar.</span><span class="sxs-lookup"><span data-stu-id="ab4de-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="ab4de-p105">Ve bu gerçekten zaten biraz fazla uzun. Yaklaşık 400 karakter en iyi uygulamadır---</span><span class="sxs-lookup"><span data-stu-id="ab4de-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ab4de-p106">İçeriğinizi hazır olduktan sonra canlı dala çeker. Daha sonra [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) gidin ve dosya adı url alanına girin. Gözden geçirilmiş ve yayımlanan Insight "Evet" diyor emin olun ve sonra güncelleştirme Kuralı'nı tıklatın. **(Bu yakında serbest portal - yeni sürümünde prettier bakar.)** 
 ![url alanı](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="ab4de-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

