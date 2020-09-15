---
title: İçerik arama sonuç yok
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680667"
---
# <a name="no-results-from-content-searchexports"></a>Içerik arama/dışarı aktarma işleminden gelen sonuçlar yok

Içerik arama/dışarı aktarma ile ilgili sorunlar, belirli bir yönetici tarafından ayarlanmış olan ve tüm yöneticilerle iletişim kurmayabilir.

Bunu çözmek için, bu soruna neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:
1. Güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanma
2. Aşağıdaki komutu çalıştırarak:
<br>$org = "yourdomain.com"
<br>Get-Karmaşıısecurityfilter-kuruluş $org