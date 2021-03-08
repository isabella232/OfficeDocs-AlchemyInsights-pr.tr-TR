---
title: Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmıyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480703"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Bir Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmıyor

Tüm grup üyelerinin e-posta almak üzere abone olduğundan emin olun. [Outlook’ta bir grubu takip etme](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36) makalesine bakın.  

Grup e-postalarına abone olmuş üyelerin ileti durumunu kontrol etmek için aşağıdaki komutu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)’de çalıştırın:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Tüm grup üyelerini Microsoft 365 grubuna gönderilen e-postaları kendi gelen kutularında alacak şekilde yapılandırmak için aşağıdaki EXO PowerShell komutunu kullanın:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Örneğin:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`