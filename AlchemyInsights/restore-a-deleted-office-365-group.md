---
title: Silinmiş Microsoft 365 grubunu geri yükleme
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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645151"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Silinmiş Microsoft 365 grubunu geri yükleme

Silinen Microsoft 365 grubunu veya Microsoft Teams'i, silinmeden önceki 30 gün içinde geri yükleyebilirsiniz.

1. Microsoft [365 yönetim merkezine](https://aka.ms/RestoreDeletedGroup) gidip silinen gruplarınız ve ekipleriniz listesinde oturum açabilirsiniz.

    **Not:** Kiracı yöneticisine veya gruplar yöneticisi rolüne atanan hesabı kullanarak oturum açın.

1. Geri yüklenecek silinmiş Microsoft 365 grubunu/Teams'i seçin ve Geri Yükle **grubu'na tıklayın.**

    Çakışan bir SMTP adresi nedeniyle grup geri yüklenebilirse, çakışmaya neden olan nesneyi bulmak ve SMTP adresini kaldırmak için aşağıdaki komutu kullanın:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Not:** Bazı durumlarda, grubun ve tüm verilerin geri yüklenebilir olması 24 saate kadar sürebilir.

    Daha fazla bilgi edinmek veya PowerShell kullanarak grupları geri yükleme hakkında bilgi edinmek için bkz. Silinmiş [Microsoft 365 grubunu geri yükleme.](https://go.microsoft.com/fwlink/?linkid=867802)