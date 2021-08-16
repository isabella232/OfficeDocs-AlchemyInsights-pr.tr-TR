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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046772"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arşiv posta kutunuz neredeyse dolu

Kullanıcı uyarıyı alırsa; **Arşiv posta kutunuz neredeyse dolu** veya arşiv posta kutusunun boyutunu artırmanız gerekiyor. Bazı ipuçları:

1. Kullanıcıya Plan 1 lisansı Exchange Online, boyutu 50 GB'tan 100 **GB'a** Exchange Online Plan 2 lisansına yükseltin.
1. Kullanıcıya önceden şu adımlar atanmışsa: **Exchange Online Plan 2 veya** Exchange Online Exchange Online Arşivleme eklentisi olan bir Exchange Online Plan 1, Otomatik Genişleyen arşivlemeyi etkinleştirmek için aşağıdaki adımları kullanın:
 
    1. [Bağlan Powershell'Exchange Online için yeni bir komutlar.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Kullanıcı için aşağıdaki komutu çalıştırın:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Kullanıcı için etkinleştirdiğini onaylamak için aşağıdaki komutu çalıştırın:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Daha fazla bilgi için bkz.:

- [Sınırsız arşivlemeyi etkinleştirme - Yönetici Yardımı - Uyumluluk Microsoft 365'| Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online sınırları - Hizmet Açıklamaları | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Farklı bir iş planı planına | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

