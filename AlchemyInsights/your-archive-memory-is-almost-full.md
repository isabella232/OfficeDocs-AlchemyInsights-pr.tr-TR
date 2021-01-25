---
title: Arşiv posta kutunuz neredeyse dolu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974667"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arşiv posta kutunuz neredeyse dolu

Kullanıcı uyarıyı alırsa; **Arşiv posta kutunuz neredeyse dolu** veya arşiv posta kutularının boyutunu artırmanız gerekirse, burada bazı ipuçları verilmiştir:

1. Kullanıcıya Exchange Online Plan 1 atanmışsa, 50 GB 'den 100GB'A kadar olan boyutu yükseltmek için **Exchange Online Plan 2** lisansına yükseltin.
1. Kullanıcıya aşağıdakilerden herhangi biri atanmış durumda: Exchange Online arşivleme eklentisi ile Exchange **Online Plan 2** veya Exchange Online Plan 1, otomatik genişletme arşivleme özelliğini etkinleştirmek için aşağıdaki adımları kullanın:.
 
    1. [Exchange Online PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Kullanıcıya aşağıdaki komutu bırakın:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Aşağıdaki komutu çalıştırıp Kullanıcı için etkinleştirildiğini doğrulayın:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Daha fazla bilgi için bkz.

- [ Sınırsız arşivlemeyi etkinleştir-Yönetici Yardımı-Microsoft 365 uyumluluğu | Microsoft belgeleri](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online sınırları-hizmet açıklamaları | Microsoft belgeleri](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Farklı bir iş planına yükselt | Microsoft belgeleri](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

