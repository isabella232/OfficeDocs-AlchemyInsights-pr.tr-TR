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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380525"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Birincil e-posta adresi ayarlamak veya kullanıcı özniteliklerini değiştirmek için

Ortamınız için dizin eşitleme etkinse, bazı kullanıcı veya nesne özniteliklerini Yönetim Merkezi'ni kullanarak değiştirilemez.
Eşzamanlı kullanıcılar ve tüm öznitelikleriyle tam olarak yönetmek için yerel active directory kullanıcıları ve grupları Yönetimi Konsolu (adsiedit.msc) kullanın.  

Alternatif olarak, tek tek kullanıcılara veya gibi ortak bu örneklerde gösterilen powershell kullanarak eşitlenen kullanıcıların özniteliklerini değiştirebilirsiniz: 
- Kümesi-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Kümesi-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test" kullanıcı"- Soyadı"Kullanıcı"-"Yönetici"Başlık-bölüm"HR"
- Kaldır-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com