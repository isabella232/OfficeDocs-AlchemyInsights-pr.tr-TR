---
title: Güçlü parola gereksinimini değiştirme
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
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070704"
---
# <a name="change-strong-password-requirement"></a>Güçlü parola gereksinimini değiştirme

Microsoft varsayılan olarak güçlü parolalar gerektirir.

PowerShell kullanarak, şu komutlarla belirli kullanıcıların güçlü parolalarını devre dışı abilirsiniz:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Tüm kullanıcıların güçlü parolalarını devre dışı bırakmak için şunları kullanın:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Parola ilkesi hakkında daha fazla bilgi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Microsoft 365'a PowerShell ile bağlanma](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell MsolUser komutları hakkında daha fazla bilgi](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
