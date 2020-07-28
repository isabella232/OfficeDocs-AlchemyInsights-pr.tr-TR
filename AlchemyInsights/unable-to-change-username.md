---
title: Kullanıcı Adı değiştirileme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440295"
---
# <a name="unable-to-change-username"></a>Kullanıcı Adı değiştirileme

Bazı durumlarda, UPN (UserPrincipalName) değişiklikleri buluta yayılmaz. Office 365 portalında doğrulama hataları alabilir veya kullanıcı adını veya e-posta adresini değiştiremeyebilirsiniz. Bu sorunu gidermek için, bu PowerShell komutunu kullanarak ManualPrincipalName'yi el ile ayarlayın.

**Örnek: Kullanıcıyı yeniden adlandır**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Bu komut davidc@contoso.com davidchew@contoso.com yeniden adlandırır.

Daha fazla bilgi için [Set-MsolUserPrincipalName'e](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)bakın.