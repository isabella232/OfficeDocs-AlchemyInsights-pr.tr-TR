---
title: eBulma dışarı aktarma aracı
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711115"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>EBulma dışarı aktarma aracı yüklenemiyor veya çalıştırılamıyor misiniz?

Arama sonuçlarını indirmek için eBulma dışarı aktarma aracı 'nı yükleyemiyor veya çalıştıramıyorsanız, aşağıdakileri denetleyin:
  
- Kullandığınız bilgisayar bu önkoşulları karşılar:

  - Windows 7 ve sonraki sürümlerin 32 veya 64-bit sürümleri

  - Microsoft .NET Framework 4.7

  - Desteklenen bir tarayıcı:

  - Microsoft Edge

    Veya

  - Internet Explorer 10 ve sonraki sürümleri

    Google Chrome ve Mozilla Firefox gibi diğer tarayıcılar desteklenmez.

- Kuruluşunuz, Azure 'da ** \* . blob.Core.Windows.net** (joker karakter, dışarı aktarma işiniz için benzersiz tanımlayıcıyı temsil eder) uç noktasına bağlanabilir.

- Microsoft 365 güvenlik Uyumluluk Merkezi 'nde dışarı aktarma rolüne atanırsınız &amp; . Varsayılan olarak bu rol yalnızca eBulma Yöneticisi rol grubuna atanır. [EBulma Izinleri atama](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)konusuna bakın.

Daha fazla bilgi için bkz: [Içerik arama sonuçlarını dışarı aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  