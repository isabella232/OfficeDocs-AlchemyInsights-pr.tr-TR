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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101322"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>eBulma Dışarı Aktarma Aracı'nı yükleye mi çalıştırasınız veya çalıştırasınız?

Arama sonuçlarını indirmek için eBulma Dışarı Aktarma Aracı'nı yükleye değil de çalıştırasanız, aşağıdaki kontrol edin:
  
- Kullanmakta olduğunuz bilgisayar şu önk önkulları karşılar:

  - 7 ve sonraki sürümlerin 32 veya 64 bit Windows sürümleri

  - Microsoft .NET Framework 4.7

  - Desteklenen bir tarayıcı:

  - Microsoft Edge

    Veya

  - Internet Explorer 10 sürümleri

    Google Chrome ve Mozilla Firefox gibi diğer tarayıcılar desteklenmez.

- Organizasyonunız Azure'daki **\* .blob.core.windows.net** uç noktasına bağlanabilirsiniz (joker karakter, dışarı aktarma işinin benzersiz bir tanımlayıcısını temsil eder).

- Güvenlik Uyumluluk Merkezi'nde Dışarı Aktarma rolüne Microsoft 365 &amp; atandı. Varsayılan olarak, bu rol yalnızca eBulma Yöneticisi rol grubuna atanır. Bkz. [eBulma izinleri atama.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Daha fazla bilgi için bkz. [İçerik Arama sonuçlarını dışarı aktarma.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

100.000'den fazla posta kutusunu dışarı aktarıyorsanız, Sonuçları dışarı aktarma:  [100.000'den](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)fazla posta kutusundan sonuçları dışarı aktarma.