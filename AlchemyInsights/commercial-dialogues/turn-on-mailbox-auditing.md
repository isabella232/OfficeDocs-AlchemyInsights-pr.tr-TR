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
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483547"
---
# <a name="turn-on-mailbox-auditing"></a>Posta kutusu denetimini açma

Tek bir kullanıcı veya kuruluşun tamamı için posta kutusu denetimini açmak için, Remote PowerShell'den aşağıdaki cmdlet'leri çalıştırın:

- **Tek kullanıcı:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Kuruluş:** Get-Mailbox -ResultSize Sınırsız -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Daha fazla bilgi edinmek için [bkz. Posta kutusu denetimini yönetme.](https://go.microsoft.com/fwlink/?linkid=2103668)