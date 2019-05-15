---
title: Modern site kök site olarak
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057791"
---
# <a name="modern-site-as-root-site"></a>Modern site kök site olarak

[Hedef sürüm](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) müşteriler artık Klasik kök sitesinde kendi SharePoint Kiracı, modern iletişim site deneyimini etkinleştirebilirsiniz.

Bu özellik, basit bir PowerShell cmdlet'ini çalıştırarak etkinleştirilebilir. PowerShell command(s) başarılı yürütülmesine kök sitesi iletişim site giriş sayfası olacaktır. PowerShell cmdlet ve özellik gereksinimleri hakkındaki ayrıntıları [Etkinleştir SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)makalesinde bulunmaktadır. 

Biz yavaş yavaş bu çıkışı, kapalı erken Mayıs 2019 yayın hedeflenen müşterilere varsayılan olarak çalışırken ve Top dışarı tüm dünyada Haziran 2019 sonuna kadar kullanılabilir olacaktır. [İleti Merkezi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) için diğer yeni özellikleri ile Modern başvurmak devam edin. 

**Önemli**: modern iletişim Site oluşturmak için Klasik kök site silmeyin. Bu Microsoft tarafından desteklenmez. Siteyi geri yüklemek veya aynı URL'de yeni bir site oluşturmak kadar kök site silindiğinde tüm SharePoint siteleri, kuruluşunuzdaki tüm kullanıcılar için erişilebilir hale getirir. 
 
 