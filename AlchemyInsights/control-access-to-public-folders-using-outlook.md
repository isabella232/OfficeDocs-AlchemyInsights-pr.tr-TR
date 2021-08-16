---
title: Klasörleri kullanarak ortak klasörlere erişimi Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032578"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Klasörleri kullanarak ortak klasörlere erişimi Outlook

Klasörleri kullanarak ortak klasörlere hangi kullanıcıların erişeni Outlook:

1. Kullanım `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Kullanıcıların e-postada ortak klasörlere erişmesine izin Outlook  
$false: Bir klasörde kullanıcının ortak klasörlere erişimini Outlook. Bu, varsayılan değerdir.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Not: Bu yordam, yalnızca Outlook istemcileri için Outlook Windows denetime sahiptir. Kullanıcılar, OWA veya klasörleri kullanarak ortak klasörlere erişmeye devam Mac için Outlook.

Daha fazla bilgi için bkz. [Denetimli Ortak Klasörlere Outlook](https://aka.ms/controlpf) Daha fazla bilgi için bkz.
