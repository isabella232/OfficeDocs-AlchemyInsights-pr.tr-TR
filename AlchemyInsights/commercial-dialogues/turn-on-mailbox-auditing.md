---
title: Posta kutusu denetimini açma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058058"
---
# <a name="turn-on-mailbox-auditing"></a>Posta kutusu denetimini açma

Tek bir kullanıcıda veya tüm kuruluşta posta kutusu denetimini açmak için, Remote PowerShell'den aşağıdaki cmdlet'leri çalıştırın:

- **Tek kullanıcı:** Set-Mailbox -Identity "Jale Dow" -AuditEnabled $true
- **Kuruluş:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Daha fazla bilgi edinmek için [bkz. Posta kutusu denetimini yönetme.](https://go.microsoft.com/fwlink/?linkid=2103668)