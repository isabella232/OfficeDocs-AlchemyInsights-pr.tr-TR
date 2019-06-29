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
# <a name="content-search-not-returning-expected-results"></a>Beklenen sonuçları döndürülüyor değil içerik arama

Office 365 güvenlik & Uyumluluk Merkezi içerik arama çalıştırıldığında, arama beklenmeyen sonuçlar alabilirsiniz. Arama sonuçlarınızı etkileyebilir şunları göz önünde bulundurun:

- **İçerik konumları ve arama koşulları**: uygun içerik konumları seçtiyseniz ve arama koşulları emin olun. (Birçok konumlar ile) büyük bir Arama çalıştırılmışsa, birden çok arama bölmeyi düşünün.

- **Kısmen dizinli öğe**: tahmini arama sonuçlarında posta kutularına gelen [kısmen öğeleri dizine](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dahil edilir. Ancak, SharePoint ve OneDrive sitelerinden kısmen dizinli öğe arama tahmine dahil edilmez.

- **Arama hataları**: çok sayıda posta kutuları (100.000 posta kutuları) ararken, arama hataları, hata kodları CS008-009 ve CS012-002 gibi alabilirsiniz). Bu durumda, yalnızca başarısız içerik konumları için aramayı yeniden deneyin. [Bu makalede](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) daha fazla bilgi için bkz.
