---
title: Içerik arama/dışarı aktarma sırasında hiçbir sonuç döndürülmedi
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680331"
---
# <a name="no-results-returned-during-content-searchexport"></a>Içerik arama/dışarı aktarma sırasında hiçbir sonuç döndürülmedi

Aşağıdaki eBulma senaryolarında sorun yaşıyorsanız:

- İçerik arama/verme işlevi veri veya beklenmeyen veriler döndürmüyor
- eBulma arama veya dışarı aktarma başarısız

Bu durum, belirli bir yönetici tarafından ayarlanan ve tüm yöneticilere iletilmedi olan uyumluluk güvenlik filtreleri nedeniyle oluşmuş olabilir.

Bunu çözmek için, bu sorunlara neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:

1. Güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanma
2. Aşağıdaki komutu çalıştırarak:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Uyumluluk güvenliği filtreleri hakkında ek bilgi için bkz: [Içerik araması Için Izinler filtreleme](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
