---
title: 1336 RecoverableItems klasörü dolu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510772"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kurtarılabilir Öğeler klasörü dolu

Exchange Online posta kutuları için, Kurtarılabilir Öğeler klasörü için varsayılan depolama sınırı 30 GB'dır. Kurtarılabilir Öğeler klasörü için depolama sınırı, posta kutusu Dava Bekletme, eDiscovery tutma veya saklama ilkesine atanmışsa otomatik olarak 100 GB'a yükseltilir.

Kurtarılabilir Öğeler klasörü depolama sınırına ulaştığında, posta kutusu işlevselliği aşağıdaki şekillerde etkilenir:

- Kullanıcı öğeleri posta kutusundan silemez.

- Yönetilen Klasör Yardımcısı, bekletme etiketine veya yönetilen klasör ayarlarına göre öğeleri silemez.

- Tek Öğe Kurtarma özelliği etkinleştirilmiş veya beklemeye alınan posta kutuları için, yazma da yazma sayfası koruma işlemi, kullanıcı tarafından düzenlenen öğelerin sürümlerini koruyamaz.

- Posta kutusu denetim günlüğü etkinleştirilmiş posta kutuları için, Kurtarılabilir Öğeler klasöründeki Denetimler alt klasörüne hiçbir posta kutusu denetim günlüğü girişi kaydedilemez.

Beklemede olmayan posta kutularında yöneticiler, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Kurtarılabilir Öğeler klasöründeki öğeleri silmek için Exchange Online PowerShell'deki komutu kullanabilir. Daha fazla bilgi için, aşağıdaki konulara bakın:

- [İletileri arama ve silme](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Arama-Posta Kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Beklemede olan posta kutuları için, yöneticilerin öğeleri Kurtarılabilir Öğeler klasöründen silmeden önce beklemeyi kaldırmaları gerekir. Daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Kurtarılabilir Öğeler klasörünün dolmasını önlemeye yardımcı olmak için yöneticiler, bekleyen posta kutuları için Kurtarılabilir Öğeler klasörünün depolama sınırını artırabilir ve öğeleri Kurtarılabilir Öğeler klasöründen kullanıcının arşiv posta kutusuna taşıyan bir posta kutusu bekletme ilkesi ayarlayabilir. Bkz. [Beklemedeki posta kutuları için Kurtarılabilir Öğeler kotasını artırın.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
