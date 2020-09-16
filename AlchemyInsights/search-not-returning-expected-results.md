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
# <a name="content-search-not-returning-expected-results"></a>İçerik araması beklenen sonuçları döndürmüyor

Microsoft 365 güvenlik & Uyumluluk Merkezi 'nden Içerik aramalarını çalıştırırken beklenmeyen arama sonuçları alabilirsiniz. Arama sonuçlarınızı etkileyebilecek aşağıdakileri göz önünde bulundurun:

- **İçerik konumları ve arama koşulları**: doğru içerik konumlarını ve arama koşullarını seçtiğinizden emin olun. Büyük bir arama çalıştırdıysanız (birçok konumda), bunu birden çok aramaya bölmeyi düşünebilirsiniz.

- **Kısmen dizinlenen öğeler**: posta kutularından  [kısmen dizinlenen öğeler](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) tahmini arama sonuçlarına eklenir. Ancak, SharePoint ve OneDrive 'daki sitelerden kısmen dizinli öğeler arama tahmininde yer alır.

- **Arama hataları**: çok sayıda posta kutusu (100.000 posta kutularıyla) ararken, CS008-009 ve CS012-002 gibi hata kodlarıyla arama hataları alabilirsiniz. Bu durumda, yalnızca başarısız içerik konumları için aramayı yeniden deneyin. Daha fazla bilgi için  [Bu makaleye](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) bakın.
