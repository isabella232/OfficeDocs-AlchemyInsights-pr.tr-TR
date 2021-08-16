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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058022"
---
# <a name="no-results-from-content-searchexports"></a>İçerik Arama/Dışarı Aktarma sonuçlarından sonuç yok

İçerik Arama/Dışarı Aktarma işlemiyle ilgili hiçbir veri döndürene sorunlar, belirli bir Yönetici tarafından kurulumu yapılan ve tüm Yöneticilere ile iletişim kurmadan dolayı belirli bir Uyumluluk Güvenlik Filtresi olabilir.

Bu sorunu çözmek için, soruna neden olacak herhangi bir Uyumluluk Güvenlik Filtresi olup olmadığını kontrol edin:
1. Bağlan ve Uyumluluk Merkezi Powershell'e
2. Aşağıdaki komutlar çalıştırın:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org