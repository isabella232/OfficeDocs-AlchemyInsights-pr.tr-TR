---
title: 1491-Search-Not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355897"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d0492-102">Beklenen sonuçları döndürülüyor değil içerik arama</span><span class="sxs-lookup"><span data-stu-id="d0492-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d0492-103">Office 365 güvenlik & Uyumluluk Merkezi içerik arama çalıştırıldığında, arama beklenmeyen sonuçlar alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d0492-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d0492-104">Arama sonuçlarınızı etkileyebilir şunları göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="d0492-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d0492-105">**İçerik konumları ve arama koşulları**: uygun içerik konumları seçtiyseniz ve arama koşulları emin olun.</span><span class="sxs-lookup"><span data-stu-id="d0492-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d0492-106">(Birçok konumlar ile) büyük bir Arama çalıştırılmışsa, birden çok arama bölmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="d0492-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d0492-107">**Kısmen dizinli öğe**: tahmini arama sonuçlarında posta kutularına gelen [kısmen öğeleri dizine](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="d0492-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d0492-108">Ancak, SharePoint ve OneDrive sitelerinden kısmen dizinli öğe arama tahmine dahil edilmez.</span><span class="sxs-lookup"><span data-stu-id="d0492-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d0492-109">**Arama hataları**: çok sayıda posta kutuları (100.000 posta kutuları) ararken, arama hataları, hata kodları CS008-009 ve CS012-002 gibi alabilirsiniz).</span><span class="sxs-lookup"><span data-stu-id="d0492-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d0492-110">Bu durumda, yalnızca başarısız içerik konumları için aramayı yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="d0492-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d0492-111">[Bu makalede](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="d0492-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
