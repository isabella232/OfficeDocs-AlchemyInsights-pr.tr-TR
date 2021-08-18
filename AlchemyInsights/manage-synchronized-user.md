---
title: Eşitlenmiş Kullanıcı Yönetme
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114804"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Birincil e-posta adresi ayar, kullanıcı özniteliklerini değiştiremiyor veya eşitlenmiş bir kullanıcı kaldır/silemiyor

Ortamınız için dizin eşitlemesi etkinleştirildiyse, bazı kullanıcı veya nesne öznitelikleri varsayılan kullanıcı veya Microsoft 365 yönetim merkezi.

Eşitlenmiş kullanıcıları ve onların tüm özniteliklerini tam olarak yönetmek için, yerel Active Directory kullanıcılarınızı ve grup yönetim konsolunuzu (adsiedit.msc) kullanın.  

Alternatif olarak, şu yaygın örneklerde gösterildiği gibi Powershell kullanarak eşitlenmiş kullanıcıların tek tek kullanıcılarını veya özniteliklerini değiştirebilirsiniz:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
