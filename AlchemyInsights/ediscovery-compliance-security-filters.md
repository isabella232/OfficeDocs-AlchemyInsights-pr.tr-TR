---
title: İçerik Arama/Dışarı Aktarma sırasında sonuç döndürül yok
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101286"
---
# <a name="no-results-returned-during-content-searchexport"></a>İçerik Arama/Dışarı Aktarma sırasında sonuç döndürül yok

Aşağıdaki eBulma senaryolarında sorun yaşıyorsanız:

- İçerik Arama/Dışarı Aktarma veri veya beklenmeyen veri sonuç vermez
- eBulma Arama veya Dışarı Aktarma başarısız

Bunun nedeni, belirli bir Yönetici tarafından kurulumu yapılan ve tüm Yöneticilere iletilen bazı Uyumluluk Güvenlik Filtreleri olabilir.

Bu sorunu çözmek için, bu sorunlara neden olacak herhangi bir Uyumluluk Güvenlik Filtresi olup olmadığını kontrol edin:

1. Bağlan ve Uyumluluk Merkezi Powershell'e
2. Aşağıdaki komutlar çalıştırın:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Uyumluluk Güvenlik Filtreleri hakkında ek bilgi için bkz. [İçerik Arama için İzin Filtreleme](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
