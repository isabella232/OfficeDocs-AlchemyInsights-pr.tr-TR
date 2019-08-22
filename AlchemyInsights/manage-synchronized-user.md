---
title: Eşzamanlı kullanıcı yönetme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542037"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Birincil e-posta adresi ayarlamak veya kullanıcı özniteliklerini değiştirmek için

Ortamınız için dizin eşitleme etkinse, Microsoft 365 Yönetim Merkezi'ni kullanarak bazı kullanıcı veya nesne öznitelikleri değiştirilemez.

Eşzamanlı kullanıcılar ve tüm öznitelikleriyle tam olarak yönetmek için yerel active directory kullanıcıları ve grupları Yönetimi Konsolu (adsiedit.msc) kullanın.  

Alternatif olarak, tek tek kullanıcılara veya gibi ortak bu örneklerde gösterilen powershell kullanarak eşitlenen kullanıcıların özniteliklerini değiştirebilirsiniz: 
- Kümesi-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Kümesi-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test" kullanıcı"- Soyadı"Kullanıcı"-"Yönetici"Başlık-bölüm"HR"
- Kaldır-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com