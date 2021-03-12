---
title: Gelişmiş av sorguları için en iyi yöntemleri uygulama
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749552"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="5edd0-102">Gelişmiş av sorguları için en iyi yöntemleri uygulama</span><span class="sxs-lookup"><span data-stu-id="5edd0-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="5edd0-103">Sonuçları daha hızlı elde etmek ve karmaşık sorguları çalıştırırken zaman aşımından kaçınmak için, şu en iyi yöntemleri uygulayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="5edd0-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="5edd0-104">Yeni sorguları deniyorum, aşırı büyük sonuç kümelerini almaktan kaçınmak için her zaman bir sınır kullanın.</span><span class="sxs-lookup"><span data-stu-id="5edd0-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="5edd0-105">Ayrıca, `count` sonuç kümesi boyutunun ilk değerlendirmesini yapmak için de kullanın.</span><span class="sxs-lookup"><span data-stu-id="5edd0-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="5edd0-106">Önce zaman filtrelerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="5edd0-106">Use time filters first.</span></span> <span data-ttu-id="5edd0-107">İdeal olan, sorgularınızı yedi günle sınırlandırma.</span><span class="sxs-lookup"><span data-stu-id="5edd0-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="5edd0-108">Sorgunun en başında, zaman filtresinin hemen ardından, verilerin büyük bir çoğunun kaldır olması beklenen filtreleri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="5edd0-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="5edd0-109">Tam belirteçleri arıyorken, bunun yerine `has` işleci `contains` kullanın.</span><span class="sxs-lookup"><span data-stu-id="5edd0-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="5edd0-110">Tüm sütunlar yerine belirli bir sütunda arama çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="5edd0-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="5edd0-111">Tabloları katılırken, önce tabloyu daha az satırla belirtin.</span><span class="sxs-lookup"><span data-stu-id="5edd0-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="5edd0-112">`project` yalnızca katıldığım tablolardan gerekli sütunlar.</span><span class="sxs-lookup"><span data-stu-id="5edd0-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="5edd0-113">Daha fazla bilgi edinmek için gelişmiş [av sorgusu en iyi yöntemlerine bakın.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="5edd0-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
