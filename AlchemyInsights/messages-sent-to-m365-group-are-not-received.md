---
title: Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051520"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Microsoft 365 grubuna gönderilen iletiler tüm üyeler tarafından alınmaz

Tüm grup üyelerinin e-postaları almak için abone olduğundan emin olun. Bkz. [Outlook'ta bir grubu takip edin.](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)  

Grup e-postalarına abone olan üyelerin ileti durumunu kontrol etmek için [EXO PowerShell'de](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)aşağıdaki komutu çalıştırın:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`