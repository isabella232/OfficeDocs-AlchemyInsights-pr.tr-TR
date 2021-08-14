---
title: Silinmiş bir grup Microsoft 365 geri yükleme
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959046"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Silinmiş bir grup Microsoft 365 geri yükleme

Silinen bir grubu veya Microsoft 365 30 gün Microsoft Teams içinde geri yükleyebilirsiniz.

1. Silinmiş [Microsoft 365 yönetim merkezi](https://aka.ms/RestoreDeletedGroup) ve ekipler listeniz listesinde oturum açmak için Kullanıcı Listesine gidin.

    **Not:** Kiracı yöneticisine veya gruplar yöneticisi rolüne atanan hesabı kullanarak oturum açın.

1. Geri yüklenecek silinmiş Microsoft 365 grubu/Teams öğesini seçin ve Grubu geri **yükle'ye tıklayın.**

    Çakışan bir SMTP adresi nedeniyle grup geri yüklenebilirse, çakışmaya neden olan nesneyi bulmak ve SMTP adresini kaldırmak için aşağıdaki komutu kullanın:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Not:** Bazı durumlarda, grubun ve tüm verilerin geri yüklenebilir olması 24 saate kadar sürebilir.

    PowerShell kullanarak grupları geri yükleme hakkında daha fazla bilgi edinmek için bkz. Silinmiş bir Grup [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)