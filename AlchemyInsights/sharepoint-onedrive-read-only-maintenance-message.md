---
title: SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620743"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint veya OneDrive kullanmaya çalışırken bakım ileti için salt okunur

Kullanıcılar, SharePoint veya OneDrive aşağıdaki senaryolardan birini kullanmaya çalışırken bir **Bakım için salt okunur** ileti alabilirsiniz. 

-   Bir etkin veya planlı bakım etkinlikleri.  Onlar için [İleti Merkezi](https://portal.office.com/adminportal/home#/messagecenter)giderek denetleyin.
-   Oluşabilecek yüksek öncelikli etkin servis olayı. [Sağlık Hizmeti](https://portal.office.com/adminportal/home#/servicehealth)için giderek herhangi danışma/olayları denetleyin.
-   Beklenmeyen olaylar nedeniyle 30 min ya da bunu daha az için son sunucularda olmuyor, küçük otomatik düzeltme kurtarma senaryosu. 
    
    Hiçbir ileti merkezi vardır veya Sağlık Hizmeti bu küçük kurtarmaları için deftere naklettiği ancak normal olarak çok yakında olmalı.

Çok az sayıda olayda yukarıda listelenen üç senaryolardan birini neden olmuştur ve hizmet geri yüklendi ancak kullanıcıların tarayıcı önbellek temizlenmiş taşınmadığından Kutlandı.

Lütfen siteye gitmeden önce tarayıcı önbelleği temizlemek deneyin.

1. Microsoft Edge tarayıcınızın **ayarlarını**seçin ve ardından **Gizlilik ve güvenlik**seçin.
2. **Clear göz**altında **temizlemek ne seçin**seçin.
3. **Tanımlama bilgileri ve kaydedilmiş Web sitesi verilerini**seçin ve **Temizle'yi**seçin.

>[!Note] 
> Bu adımlar, Mozilla Firefox veya Google Chrome gibi başka tarayıcıları kullanırken, farklı olabilir.

>[!Note] 
> SharePoint sitesi veya OneDrive yeni InPrivate penceresinde açmak için başka bir seçenek olacaktır.