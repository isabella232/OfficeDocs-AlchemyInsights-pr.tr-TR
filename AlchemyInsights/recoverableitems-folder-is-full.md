---
title: 1336 RecoverableItems klasörü dolu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776416"
---
# <a name="the-recoverable-items-folder-is-full"></a>Kurtarılabilir öğeleri klasörü dolu

Office 365'te çevrimiçi Exchange posta kutuları için kurtarılabilir öğeleri klasör için varsayılan depolama sınırı 30 GB'dır. Posta kutusu dava tutun, eBulma tutun yerleştirilir veya bir Office 365 bekletme ilkesine atandığından kurtarılabilir öğeleri klasör için depolama sınırı 100 GB'a otomatik olarak artırılır.
  
Kurtarılabilir öğeleri klasör depolama sınırına ulaştığında, posta kutusu işlevselliği aşağıdaki şekillerde etkilenir:
  
- Kullanıcının posta kutusundan öğeler silinemiyor.
    
- Yönetilen Klasör Yardımcısı bekletme etiket veya yönetilen klasör ayarları temel öğelerini silemezsiniz.
    
- Tek öğe kurtarma etkinleştirilmiş veya beklemeye alınan posta kutuları için kopyası üzerinde yazma sayfa koruma işlemi kullanıcı tarafından düzenlenen öğelerin sürümleri korunamaz.
    
- Denetim günlüğü etkin posta kutunuz posta kutuları için posta kutusu denetim günlük girdisi denetimleri alt kurtarılabilir öğeler klasörüne kaydedilebilir.
    
Beklemede olmayan posta kutuları için admins kullanabilirsiniz `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kurtarılabilir öğeleri klasörü'ndeki öğeleri silmek için Exchange Online PowerShell komutunu. Daha fazla bilgi için, aşağıdaki konulara bakın: 
  
- [Arama ve iletileri silme](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Posta kutusu arama](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Beklemede olan posta kutuları için admins tutma bunlar kurtarılabilir öğeleri klasörden silinen öğeleri için önce kaldırmanız gerekir. Daha fazla bilgi için bkz: [Klasör bulut tabanlı posta kutularının üzerinde tutun kurtarılabilir öğeleri öğeleri silmek](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Kurtarılabilir öğeleri klasör tam olmasını önlemek için Yöneticiler kurtarılabilir klasör için posta kutuları üzerinde tutun ve kullanıcının arşive kurtarılabilir Öğeler klasöründeki öğeleri taşıyan bir posta kutusu bekletme ilkesini ayarlamak öğelerin depolama sınırını artırabilirsiniz posta kutusu. [Kurtarılabilir öğeleri üzerinde posta kutuları için kota tutun artırmak](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)bakın.
  

