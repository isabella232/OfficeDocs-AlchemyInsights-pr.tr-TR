---
title: Güçlü Parola Gereksinimini Değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286298"
---
# <a name="change-strong-password-requirement"></a>Güçlü parola gereksinimini değiştirme

Microsoft varsayılan olarak güçlü parolalar gerektirir. 

PowerShell'i kullanarak, bu komutla belirli kullanıcılar için güçlü parolaları devre dışı kullanabilirsiniz:<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [Parola ilkesi hakkında daha fazla bilgi](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell ile Office 365'e bağlanma](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell MsolUser komutları hakkında daha fazla bilgi](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Tek bir kullanıcının parolasını süresi hiç dolmayacak şekilde ayarlama](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
