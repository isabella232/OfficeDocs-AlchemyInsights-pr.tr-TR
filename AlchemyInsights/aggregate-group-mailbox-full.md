---
title: Microsoft 365 grubuna gönderilen e-posta için AggregateGroupMailbox tam NDR alındı
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722076"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Microsoft 365 grubuna gönderilen e-posta için AggregateGroupMailbox tam NDR alındı

Toplu grup posta kutusuna gönderilen e-postaları sessizce bırakmak için Exchange aktarma kuralı oluşturmak için aşağıdaki EXO kabuğu komutunu kullanın:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> **-Sentadresindeki** SMTP adresini kiracınızdaki toplu grup posta kutusunun SMTP adresiyle değiştirin. Alınan NDR 'den toplam grup posta kutusunun SMTP adresini alabilirsiniz.



