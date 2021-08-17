---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052730"
---
# <a name="content-search-not-returning-expected-results"></a>İçerik Arama beklenen sonuçları döndürlenmiyor

Uyumluluk Merkezi'nde İçerik Microsoft 365'& çalıştırmaya devam ediyorsanız, beklenmeyen arama sonuçlarıyla karşılaşabilirsiniz. Arama sonuçlarınızı etkileyebilecek aşağıdaki şeyleri göz önünde bulundurarak:

- **İçerik konumları ve arama koşulları:** İçerik konumlarını ve arama koşullarını doğru seçtiğinizden emin olun. Büyük bir arama yaptıysanız (birçok konumu varsa), birden çok aramaya bölmeyi göz önünde bulundurabilirsiniz.

- **Kısmen dizine alan öğeler**:  [Posta kutularından](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kısmen dizine alan öğeler, tahmini arama sonuçlarına dahil edilir. Bununla birlikte, SharePoint ve OneDrive sitelerden kısmen dizine alınan öğeler arama tahmine dahil değildir.

- Arama **hataları:** Çok fazla sayıda posta kutusunda (100.000'den fazla posta kutusu) arama sırasında, CS008-009 ve CS012-002 gibi hata kodlarıyla arama hataları alabilirsiniz. Bu durumda, yalnızca başarısız içerik konumları için arama işlemini yeniden deneyin. Daha  [fazla bilgi için](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) bu makaleye bakın.
