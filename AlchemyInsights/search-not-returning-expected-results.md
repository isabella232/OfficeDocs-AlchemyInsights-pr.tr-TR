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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510592"
---
# <a name="content-search-not-returning-expected-results"></a>İçerik Arama beklenen sonuçları döndürmez

Microsoft 365 güvenlik & Uyumluluk Merkezi'nden İçerik Aramaları çalıştırırken beklenmeyen arama sonuçları alabilirsiniz. Arama sonuçlarınızı etkileyebilecek aşağıdaki şeyleri göz önünde bulundurun:

- **İçerik konumları ve arama koşulları**: Uygun içerik konumlarını ve arama koşullarını seçtiğinizden emin olun. Büyük bir arama (birçok konumla) çalıştırdıysanız, birden çok aramaya bölmeyi düşünün.

- **Kısmen dizine eklenmiş öğeler**: Posta kutularından [kısmen dizine eklenmiş öğeler,](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) tahmini arama sonuçlarına dahil edilir. Ancak, SharePoint ve OneDrive'daki sitelerden kısmen dizine eklenmiş öğeler arama tahminine dahil değildir.

- **Arama hataları**: Çok sayıda posta kutusu (100.000'den fazla posta kutusu) arama yaparken, CS008-009 ve CS012-002 gibi hata kodlarıyla arama hataları alabilirsiniz. Bu durumda, aramayı yalnızca başarısız içerik konumları için yeniden deneyin. Daha fazla bilgi için [bu makaleye](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) bakın.
