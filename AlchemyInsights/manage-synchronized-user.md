---
title: Senkronize Kullanıcıyı Yönetme
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407370"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Birincil e-posta adresini ayarlayamıyor, kullanıcı özniteliklerini değiştiremiyor veya senkronize edilmiş bir kullanıcıyı kaldıramıyor/silemiyor

Ortamınız için dizin eşitlemesi etkinleştirilmişse, Microsoft 365 yönetici merkezi kullanılarak bazı kullanıcı veya nesne öznitelikleri değiştirilemez.

Senkronize kullanıcıları ve tüm özniteliklerini tam olarak yönetmek için yerel etkin dizin kullanıcılarınızı ve grup yönetim konsolunuzu (adsiedit.msc) kullanın.  

Alternatif olarak, bu yaygın örneklerde gösterildiği gibi powershell kullanarak senkronize kullanıcılar için tek tek kullanıcıları veya özniteliklerini değiştirebilirsiniz: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
