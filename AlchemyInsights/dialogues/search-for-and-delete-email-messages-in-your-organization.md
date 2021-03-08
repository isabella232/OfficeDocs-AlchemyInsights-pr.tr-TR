---
title: Kuruluş içinde e-posta iletilerini arama ve silme
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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527274"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Kuruluş içinde e-posta iletilerini arama ve silme

Şu adımları izleyin:

1. Genel yönetici değilseniz, iletileri aramak için hesabınız **eBulma Yöneticisi** rol grubuna veya Uyumluluk Arama yönetimi **rolüne eklenmiştir.** İletileri silmek için, Kuruluş Yönetimi rol grubuna **veya Arama** ve Temizleme yönetimi **rolüne katılmanız gerekir.** Bu rollere izinler Güvenlik ve [uyumluluk & atanır.](https://protection.office.com)
2. [Silinecek iletiyi](https://docs.microsoft.com/office365/securitycompliance/content-search) bulmak için içerik araması oluşturun.
3. [Güvenlik ve Uyumluluk & PowerShell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) MFA kullanıyorsanız, şu yönergelere bakın: Çok faktörlü kimlik doğrulamasını & Güvenlik merkezi [PowerShell'e bağlanma](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. İletiyi silin: `New-ComplianceSearchAction` cmdlet'i çalıştırarak iletiyi silin. Silinen iletiler kullanıcının Kurtarılabilir Öğeler klasörüne taşınır. Örnek komut için [3. Adıma bakın: İletiyi silme.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
