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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061776"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kurtarılabilir Öğeler klasörü dolu

Daha Exchange Online için, Kurtarılabilir Öğeler klasörü için varsayılan depolama sınırı 30 GB'tır. Posta kutusu Mahkeme Tutma, eBulma bekletmeye yerleştirilirse veya bir bekletme ilkesine atanmışsa, Kurtarılabilir Öğeler klasörünün depolama sınırı otomatik olarak 100 GB'ye artırılır.

Kurtarılabilir Öğeler klasörü depolama sınırına ulaştığında, posta kutusu işlevselliği aşağıdaki şekillerde etkilenir:

- Kullanıcı posta kutusundan öğeleri silemez.

- Yönetilen Klasör Yardımcısı bekletme etiketi veya yönetilen klasör ayarlarına göre öğeleri silemez.

- Tek Öğe Kurtarma'nın etkin olduğu veya yerine konan posta kutuları için, bir kopya üzerine yazma sayfa koruma işlemi kullanıcı tarafından düzenlenen öğelerin sürümlerini tutılamaz.

- Posta kutusu denetim günlüğünün etkin olduğu posta kutularında, Kurtarılabilir Öğeler klasöründeki Denetimler alt klasörüne hiçbir posta kutusu denetim günlüğü girdisi kaydedilemez.

Tutulamaz durumdaki posta kutuları için yöneticiler Kurtarılabilir Öğeler klasöründeki öğeleri silmek Exchange Online PowerShell'de bu `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komutu kullanabilir. Daha fazla bilgi için, aşağıdaki konulara bakın:

- [İletileri arama ve silme](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Arama-Posta Kutusu](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Kurtarılabilir Öğeler klasöründeki öğeleri silebilirler. Daha fazla bilgi için [bkz. Bulut tabanlı posta kutularının Kurtarılabilir](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)Öğeler klasöründeki öğeleri tutma .

Kurtarılabilir Öğeler klasörünün dolu olmalarını önlemeye yardımcı olmak için, yöneticiler posta kutuları için Kurtarılabilir Öğeler klasörünün depolama sınırını artırabilir ve öğeleri Kurtarılabilir Öğeler klasöründen kullanıcının arşiv posta kutusuna taşırken bir posta kutusu bekletme ilkesi ayarlanabilir. Bkz. [Durumdaki posta kutuları için Kurtarılabilir Öğe kotasını artırma.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
