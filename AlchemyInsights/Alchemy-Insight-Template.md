---
title: Dosya adı ile aynı en iyisidir
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800065"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="38c04-102">Gerekli Alchemy başlık H1, H2's çalışmaz.</span><span class="sxs-lookup"><span data-stu-id="38c04-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="38c04-103">En iyi yöntemleri ve yönergeleri Alchemy yazmak için:</span><span class="sxs-lookup"><span data-stu-id="38c04-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="38c04-104">**Klasörlerde Alchemy görüşleri geçirmeyin**- Bu url yapısı kesecektir.</span><span class="sxs-lookup"><span data-stu-id="38c04-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="38c04-105">Biz bu düzeltme içine bakıyorsunuzdur.</span><span class="sxs-lookup"><span data-stu-id="38c04-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="38c04-106">Küçük harfli dosya adlarını boşluk için tire ile dosyalar **AlchemyInsights** klasöründe olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="38c04-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="38c04-107">***how-to-enable-dava-tutun***.</span><span class="sxs-lookup"><span data-stu-id="38c04-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="38c04-108">Kural kimliği veya demet kimliği [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) ms.custom alanına dahil edersiniz.</span><span class="sxs-lookup"><span data-stu-id="38c04-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="38c04-109">ex.</span><span class="sxs-lookup"><span data-stu-id="38c04-109">ex.</span></span> <span data-ttu-id="38c04-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="38c04-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="38c04-111">Meta verileri geri kalanı bu dosyanın en üstünde, şablon olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="38c04-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="38c04-112">[Alchemy ortak portalı](https://alchemyportal.azurewebsites.net)bölümüne gidin **Müşteri Insight Başlık:** ve H1 başlığınızın Insight için işaret eden bir başlangıç olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="38c04-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="38c04-113">Üstünde sahip tek bir H1 görüşleri Alchemy olmalıdır veya üretimde kesintiye uğrar.</span><span class="sxs-lookup"><span data-stu-id="38c04-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="38c04-114">H2s, bunu kullanmak **Kalın** veya ayrı bölümler belirtmek için diğer kuralları işlemek yoktur.</span><span class="sxs-lookup"><span data-stu-id="38c04-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="38c04-115">Ardından, gövde metni Alchemy kural sayfanın müşteri görüşleri bölümünde taslak malzeme kullanarak doldurun</span><span class="sxs-lookup"><span data-stu-id="38c04-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="38c04-116">Madde işaretli listeler ince</span><span class="sxs-lookup"><span data-stu-id="38c04-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="38c04-117">Çok numaralı listeler</span><span class="sxs-lookup"><span data-stu-id="38c04-117">Numbered lists too</span></span>
    1. <span data-ttu-id="38c04-118">**Kalın** ve *İtalik* a-ok</span><span class="sxs-lookup"><span data-stu-id="38c04-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="38c04-119">Bağlantıları her zaman olması gerekir ya da **"Bağlantılar Web" / dış** veya **UI öğelerine derin bağlantılar**, değil iç bağlantılar.</span><span class="sxs-lookup"><span data-stu-id="38c04-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="38c04-120">Resim şu anda resmi olarak desteklenmez, ancak bu yol haritası üzerinde.</span><span class="sxs-lookup"><span data-stu-id="38c04-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="38c04-121">Ve bu gerçekten zaten biraz fazla uzun.</span><span class="sxs-lookup"><span data-stu-id="38c04-121">And this is really already a bit too long.</span></span> <span data-ttu-id="38c04-122">Yaklaşık 400 karakter en iyi uygulamadır---</span><span class="sxs-lookup"><span data-stu-id="38c04-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="38c04-123">İçeriğinizi hazır olduktan sonra canlı dala çeker.</span><span class="sxs-lookup"><span data-stu-id="38c04-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="38c04-124">Daha sonra [Alchemy ortak portalı](https://alchemyportal.azurewebsites.net) gidin ve dosya adı url alanına girin.</span><span class="sxs-lookup"><span data-stu-id="38c04-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 