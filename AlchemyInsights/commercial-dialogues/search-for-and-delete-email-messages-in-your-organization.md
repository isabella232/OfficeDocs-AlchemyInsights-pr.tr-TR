---
title: Organizasyonda e-posta iletilerini arama ve silme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948903"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Organizasyonda e-posta iletilerini arama ve silme

Şu adımları izleyin:

1. Genel yönetici değilseniz, hesabınızla ilgili iletileri aramak için **eBulma** Yöneticisi rol grubuna veya Uyumluluk Arama yönetimi **rolüne eklenmiştir.** İletileri silmek için, Kuruluş Yönetimi rol grubuna **veya** Arama ve Temizleme **yönetim rolüne katılmanız gerekir.** Bu rollerin izinleri Güvenlik ve uyumluluk [& atanır.](https://protection.office.com)
2. [Silinecek iletiyi](https://docs.microsoft.com/office365/securitycompliance/content-search) bulmak için içerik araması oluşturun.
3. [Bağlan ve Uyumluluk & PowerShell'e.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) MFA kullanıyorsanız, şu yönergelere bakın: Multi-Factor Authentication Bağlan Güvenlik & Uyumluluk Merkezi [PowerShell'e kadar olan her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) şey
4. İletiyi silin: İletiyi `New-ComplianceSearchAction` silmek için cmdlet'i çalıştırın. Silinen iletiler bir kullanıcının Kurtarılabilir Öğeler klasörüne taşınır. Örnek bir komut için bkz. [3. Adım: İletiyi silme.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
