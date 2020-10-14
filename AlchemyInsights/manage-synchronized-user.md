---
title: Eşitlenmiş kullanıcıyı yönetme
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451420"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Birincil e-posta adresi ayarlanamıyor, Kullanıcı öznitelikleri değiştirilemiyor veya eşitlenmiş kullanıcıyı kaldırın/silin

Ortamınızda dizin eşitlemesi etkinleştirilmişse, bazı Kullanıcı veya nesne öznitelikleri Microsoft 365 Yönetim Merkezi kullanılarak değiştirilemez.

Eşitlenen kullanıcıları ve tüm özniteliklerini tümüyle yönetmek için yerel Active Directory Kullanıcıları ve grupları yönetim konsolunuzu (Adsiedit. msc) kullanın.  

Alternatif olarak, aşağıdaki yaygın örneklerde gösterildiği gibi PowerShell kullanarak eşitlenmiş kullanıcılar için tek tek kullanıcıları veya öznitelikleri değiştirebilirsiniz:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
