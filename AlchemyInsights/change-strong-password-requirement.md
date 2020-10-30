---
title: Güçlü parola gereksinimini değiştirme
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804443"
---
# <a name="change-strong-password-requirement"></a>Güçlü parola gereksinimini değiştirme

Microsoft, varsayılan olarak güçlü parolalar gerektirir.

PowerShell kullanarak, bu komutları kullanarak belirli kullanıcıların güçlü parolalarını devre dışı bırakabilirsiniz:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Tüm kullanıcıların güçlü parolalarını devre dışı bırakmak için şunları kullanın:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Parola ilkesi hakkında daha fazla bilgi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell ile Microsoft 365 'e bağlanma](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell Msolkullanıcı komutlarıyla ilgili daha fazla bilgi](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
