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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777697"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Birincil e-posta adresi ayarlanamıyor, Kullanıcı öznitelikleri değiştirilemiyor veya eşitlenmiş kullanıcıyı kaldırın/silin

Ortamınızda dizin eşitlemesi etkinleştirilmişse, bazı Kullanıcı veya nesne öznitelikleri Microsoft 365 Yönetim Merkezi kullanılarak değiştirilemez.

Eşitlenen kullanıcıları ve tüm özniteliklerini tümüyle yönetmek için yerel Active Directory Kullanıcıları ve grupları yönetim konsolunuzu (Adsiedit. msc) kullanın.  

Alternatif olarak, aşağıdaki yaygın örneklerde gösterildiği gibi PowerShell kullanarak eşitlenmiş kullanıcılar için tek tek kullanıcıları veya öznitelikleri değiştirebilirsiniz: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
