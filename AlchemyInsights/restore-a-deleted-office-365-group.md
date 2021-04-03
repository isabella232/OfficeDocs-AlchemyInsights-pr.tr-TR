---
title: Silinmiş bir Microsoft 365 grubunu geri yükleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505730"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Silinmiş bir Microsoft 365 grubunu geri yükleme

Silinen Microsoft 365 grubunu veya Microsoft Teams'i silme işleminin ardından 30 gün içinde geri yükleyebilirsiniz.

1. Microsoft 365 yönetim merkezinde oturum açma ve silinen grupları ve ekiplerin listesini yapmak [için, Microsoft 365 yönetim merkezine gidin.](https://aka.ms/RestoreDeletedGroup)

    **Not:** Kiracı yöneticisine veya gruplar yöneticisi rolüne atanan hesabı kullanarak oturum açın.

1. Geri yüklenecek silinmiş Microsoft 365 grubunu/Teams'i seçin ve Geri Yükle **grubuna tıklayın.**

    Çakışan bir SMTP adresi nedeniyle grup geri yüklenebilirse, çakışmaya neden olan nesneyi bulmak ve SMTP adresini kaldırmak için aşağıdaki komutu kullanın:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Not:** Bazı durumlarda, grubun ve tüm verilerin geri yüklenebilir olması 24 saat kadar sürebilir.

    Daha fazla bilgi edinmek veya PowerShell kullanarak grupları geri yükleme hakkında bilgi edinmek için, [bkz. Silinmiş Microsoft 365 grubunu](https://go.microsoft.com/fwlink/?linkid=867802)geri yükleme.