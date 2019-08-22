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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516799"
---
# <a name="no-results-from-content-searchexports"></a>Gelen içerik arama/dışarı sonuç

Kur tarafından belirli bir yönetim ve tüm Yöneticiler grubuna Kurulmuyor, belirli uyumluluk güvenlik filtresi nedeniyle sorunlar ile içerik arama/herhangi veri döndürmek değil dışarı olabilir.

Bu sorunu gidermek için bu neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:
1. Güvenlik ve Uyumluluk Merkezi Powershell bağlanmak
2. Aşağıdaki commandlet'lerini çalıştırın:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org organizasyon