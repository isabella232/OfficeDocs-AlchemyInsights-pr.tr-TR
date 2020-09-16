---
title: 1491-arama sonuç-sonuç-beklenen-sonuç
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740494"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e3bfe-102">İçerik araması beklenen sonuçları döndürmüyor</span><span class="sxs-lookup"><span data-stu-id="e3bfe-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e3bfe-103">Microsoft 365 güvenlik & Uyumluluk Merkezi 'nden Içerik aramalarını çalıştırırken beklenmeyen arama sonuçları alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e3bfe-104">Arama sonuçlarınızı etkileyebilecek aşağıdakileri göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="e3bfe-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e3bfe-105">**İçerik konumları ve arama koşulları**: doğru içerik konumlarını ve arama koşullarını seçtiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e3bfe-106">Büyük bir arama çalıştırdıysanız (birçok konumda), bunu birden çok aramaya bölmeyi düşünebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e3bfe-107">**Kısmen dizinlenen öğeler**: posta kutularından  [kısmen dizinlenen öğeler](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) tahmini arama sonuçlarına eklenir.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e3bfe-108">Ancak, SharePoint ve OneDrive 'daki sitelerden kısmen dizinli öğeler arama tahmininde yer alır.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e3bfe-109">**Arama hataları**: çok sayıda posta kutusu (100.000 posta kutularıyla) ararken, CS008-009 ve CS012-002 gibi hata kodlarıyla arama hataları alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e3bfe-110">Bu durumda, yalnızca başarısız içerik konumları için aramayı yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e3bfe-111">Daha fazla bilgi için  [Bu makaleye](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) bakın.</span><span class="sxs-lookup"><span data-stu-id="e3bfe-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
