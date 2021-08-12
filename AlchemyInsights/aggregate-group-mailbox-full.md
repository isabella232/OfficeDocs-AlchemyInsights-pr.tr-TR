---
title: Toplama GrubuMailbox, Bir Grup Kullanıcı Grubuna gönderilen e-posta için Microsoft 365 NDR alındı
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951873"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Toplama GrubuMailbox, Bir Grup Kullanıcı Grubuna gönderilen e-posta için Microsoft 365 NDR alındı

Toplam grup posta kutusuna gönderilen e-postaları sessiz Exchange bir aktarım kuralı oluşturmak için aşağıdaki EXO Shell komutunu kullanın:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> **-SentTo'daki** SMTP adresini kiracılı toplu grup posta kutusunun SMTP adresiyle değiştirin. NDR'nin aldığı toplu grup posta kutusunun SMTP adresini edinebilirsiniz.



