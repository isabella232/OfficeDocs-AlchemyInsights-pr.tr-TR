---
title: İçerik Arama Sonucu Yok
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816868"
---
# <a name="no-results-from-content-searchexports"></a>İçerik Arama/Dışarı Aktarma sonuçlarından sonuç yok

İçerik Arama/Dışarı Aktarma işlemiyle ilgili hiçbir veri döndürene sorunlar, belirli bir Yönetici tarafından kurulumu yapılan ve tüm Yöneticilere ile iletişim kurmadan dolayı belirli bir Uyumluluk Güvenlik Filtresi olabilir.

Bu sorunu çözmek için, soruna neden olacak herhangi bir Uyumluluk Güvenlik Filtresi olup olmadığını kontrol edin:
1. Güvenlik ve Uyumluluk Merkezi Powershell'e bağlanma
2. Aşağıdaki komutlar çalıştırın:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org