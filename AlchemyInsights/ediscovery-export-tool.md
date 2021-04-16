---
title: eBulma dışarı aktarma aracı
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814608"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>eBulma Dışarı Aktarma Aracı'nı yükleye mi çalıştırasınız veya çalıştırasınız?

Arama sonuçlarını indirmek için eBulma Dışarı Aktarma Aracı'nı yükleye değil de çalıştırasanız, aşağıdaki kontrol edin:
  
- Kullanmakta olduğunuz bilgisayar şu önk önkulları karşılar:

  - Windows 7 ve sonraki sürümlerin 32 veya 64 bit sürümleri

  - Microsoft .NET Framework 4.7

  - Desteklenen bir tarayıcı:

  - Microsoft Edge

    Veya

  - Internet Explorer 10 ve sonraki sürümleri

    Google Chrome ve Mozilla Firefox gibi diğer tarayıcılar desteklenmez.

- Organizasyonunız Azure'daki **\* .blob.core.windows.net** uç noktasına bağlanabilirsiniz (joker karakter, dışarı aktarma işinin benzersiz bir tanımlayıcısını temsil eder).

- Microsoft 365 Güvenlik Uyumluluk Merkezi'nde Dışarı Aktarma &amp; rolüne atandık. Varsayılan olarak, bu rol yalnızca eBulma Yöneticisi rol grubuna atanır. Bkz. [eBulma izinleri atama.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Daha fazla bilgi için bkz. [İçerik Arama sonuçlarını dışarı aktarma.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

100.000'den fazla posta kutusunu dışarı aktarıyorsanız, Sonuçları dışarı aktarma:  [100.000'den](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)fazla posta kutusundan sonuçları dışarı aktarma.