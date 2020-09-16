---
title: 1336 RecoverableItems klasörü dolu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741287"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kurtarılabilir Öğeler klasörü dolu

Exchange Online posta kutularında, Kurtarılabilir Öğeler klasörünün varsayılan depolama sınırı 30 GB 'dir. Posta kutusu, bir bekletme ilkesine veya bir bekletme ilkesine atanmışsa, Kurtarılabilir Öğeler klasörünün depolama sınırı 100 GB olarak otomatik olarak artırılır.

Kurtarılabilir Öğeler klasörü depolama sınırına ulaştığında, posta kutusu işlevi aşağıdaki yollarla etkilenir:

- Kullanıcı posta kutusundan öğeleri silemez.

- Yönetilen klasör Yardımcısı, saklama etiketine veya yönetilen klasör ayarlarına dayalı olarak öğeleri silemez.

- Tek öğe kurtarması etkinleştirilmiş veya beklemeye konan posta kutuları için, yazma sayfası koruma süreci Kullanıcı tarafından düzenlenen öğelerin sürümlerini sürdüremez.

- Posta kutusu denetim günlüğü etkin olan posta kutularında, Kurtarılabilir Öğeler klasöründeki denetimler alt klasörüne posta kutusu denetim günlüğü girdileri kaydedilemez.

Tutulmayan posta kutuları için, Yöneticiler, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Kurtarılabilir Öğeler klasöründeki öğeleri silmek Için Exchange Online PowerShell 'deki komutu kullanabilirler. Daha fazla bilgi için, aşağıdaki konulara bakın:

- [İletileri arama ve silme](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Arama-posta kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Beklemede olan posta kutuları için, yöneticilerin Kurtarılabilir Öğeler klasöründeki öğeleri silinebilmesi için önce tutmayı kaldırması gerekir. Daha fazla bilgi için, [bulut tabanlı posta kutularının Kurtarılabilir Öğeler klasöründeki öğeleri silme](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)konusuna bakın.

Kurtarılabilir Öğeler klasörünün tam olmasını engellemeye yardımcı olmak için, Yöneticiler, posta kutuları için Kurtarılabilir Öğeler klasörünün depolama sınırını artırıp, Kurtarılabilir Öğeler klasöründeki öğeleri kullanıcının arşiv posta kutusuna taşıyan bir posta kutusu bekletme ilkesi ayarlayabilir. [Posta kutuları Için Kurtarılabilir Öğeler kotasını arttırın](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
