---
title: İçeriği arama sonucu yok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800666"
---
# <a name="no-results-from-content-searchexports"></a>Gelen içerik arama/dışarı sonuç

Kur tarafından belirli bir yönetim ve tüm Yöneticiler grubuna Kurulmuyor, belirli uyumluluk güvenlik filtresi nedeniyle sorunlar ile içerik arama/herhangi veri döndürmek değil dışarı olabilir.

Bu sorunu gidermek için bu neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:
1. Güvenlik ve Uyumluluk Merkezi Powershell bağlanmak
2. Aşağıdaki commandlet'lerini çalıştırın:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org organizasyon