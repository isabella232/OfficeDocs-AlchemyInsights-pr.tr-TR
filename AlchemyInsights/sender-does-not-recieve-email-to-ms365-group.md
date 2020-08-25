---
title: Gönderen, Microsoft 365 grubuna gönderilen e-postayı almıyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872268"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Gönderen, Microsoft 365 grubuna gönderilen e-postayı almıyor

Varsayılan olarak, e-posta iletisinin göndereni Microsoft 365 grubuna, gönderen grubun bir üyesi olsa bile iletinin bir kopyasını gelen kutularına almaz.

Gönderenin, Microsoft 365 grubuna gönderdikleri her e-postanın bir kopyasını almasını sağlamak için bu EXO PowerShell komutunu kullanın:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Tüm posta kutularının ayarlarını aynı anda etkinleştirmek için:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Not** Bu ayarda yapılan değişikliklerin etkinleşmesi için bir saate kadar sürer.