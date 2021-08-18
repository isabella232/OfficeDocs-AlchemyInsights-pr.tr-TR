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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315930"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Toplama GrubuMailbox, Bir Grup Kullanıcı Grubuna gönderilen e-posta için Microsoft 365 NDR alındı

Toplam grup posta kutusuna gönderilen e-postaları sessiz Exchange bir aktarım kuralı oluşturmak için aşağıdaki EXO Shell komutunu kullanın:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Not:** **-SentTo'daki** SMTP adresini kiracılı toplu grup posta kutusunun SMTP adresiyle değiştirin. NDR'nin aldığı toplu grup posta kutusunun SMTP adresini edinebilirsiniz.



