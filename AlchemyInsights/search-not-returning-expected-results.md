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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383855"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="916ae-102">Beklenen sonuçları döndürülüyor değil içerik arama</span><span class="sxs-lookup"><span data-stu-id="916ae-102">Content Search not returning expected results</span></span>

<span data-ttu-id="916ae-103">Office 365 güvenlik & Uyumluluk Merkezi içerik arama çalıştırıldığında, arama beklenmeyen sonuçlar alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="916ae-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="916ae-104">Arama sonuçlarınızı etkileyebilir şunları göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="916ae-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="916ae-105">**İçerik konumları ve arama koşulları**: uygun içerik konumları seçtiyseniz ve arama koşulları emin olun.</span><span class="sxs-lookup"><span data-stu-id="916ae-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="916ae-106">(Birçok konumlar ile) büyük bir Arama çalıştırılmışsa, birden çok arama bölmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="916ae-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="916ae-107">**Kısmen dizinli öğe**: tahmini arama sonuçlarında posta kutularına gelen [kısmen öğeleri dizine](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dahil edilir.</span><span class="sxs-lookup"><span data-stu-id="916ae-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="916ae-108">Ancak, SharePoint ve OneDrive sitelerinden kısmen dizinli öğe arama tahmine dahil edilmez.</span><span class="sxs-lookup"><span data-stu-id="916ae-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="916ae-109">**Arama hataları**: çok sayıda posta kutuları (100.000 posta kutuları) ararken, arama hataları, hata kodları CS008-009 ve CS012-002 gibi alabilirsiniz).</span><span class="sxs-lookup"><span data-stu-id="916ae-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="916ae-110">Bu durumda, yalnızca başarısız içerik konumları için aramayı yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="916ae-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="916ae-111">[Bu makalede](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="916ae-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
