---
title: 1491-search-not-return-beklenen-sonuçlar
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709247"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="9ad69-102">İçerik Arama beklenen sonuçları döndürmez</span><span class="sxs-lookup"><span data-stu-id="9ad69-102">Content Search not returning expected results</span></span>

<span data-ttu-id="9ad69-103">Microsoft 365 güvenlik & Uyumluluk Merkezi'nden İçerik Aramaları çalıştırırken beklenmeyen arama sonuçları alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9ad69-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="9ad69-104">Arama sonuçlarınızı etkileyebilecek aşağıdaki şeyleri göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="9ad69-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="9ad69-105">**İçerik konumları ve arama koşulları**: Uygun içerik konumlarını ve arama koşullarını seçtiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ad69-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="9ad69-106">Büyük bir arama (birçok konumla) çalıştırdıysanız, birden çok aramaya bölmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="9ad69-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="9ad69-107">**Kısmen dizine eklenmiş öğeler**: Posta kutularından [kısmen dizine eklenmiş öğeler,](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) tahmini arama sonuçlarına dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="9ad69-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="9ad69-108">Ancak, SharePoint ve OneDrive'daki sitelerden kısmen dizine eklenmiş öğeler arama tahminine dahil değildir.</span><span class="sxs-lookup"><span data-stu-id="9ad69-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="9ad69-109">**Arama hataları**: Çok sayıda posta kutusu (100.000'den fazla posta kutusu) arama yaparken, CS008-009 ve CS012-002 gibi hata kodlarıyla arama hataları alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9ad69-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="9ad69-110">Bu durumda, aramayı yalnızca başarısız içerik konumları için yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="9ad69-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="9ad69-111">Daha fazla bilgi için [bu makaleye](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) bakın.</span><span class="sxs-lookup"><span data-stu-id="9ad69-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
