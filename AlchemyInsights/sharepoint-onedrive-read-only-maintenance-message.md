---
title: SharePoint veya OneDrive'ı kullanmaya çalışırken Yalnızca Bakım için Okuma iletisi
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051301"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint veya OneDrive'ı kullanmaya çalışırken Yalnızca Bakım için Okuma iletisi

Kullanıcılar, aşağıdaki senaryolardan biri için SharePoint veya OneDrive'ı kullanmaya çalışırken **Yalnızca Bakım için** Salt Okuma iletisi alabilir. 

-   Planlı veya etkin bir bakım faaliyeti.  [İleti Merkezi'ne](https://portal.office.com/adminportal/home#/messagecenter)yönlendirerek bunları kontrol edin.
-   Meydana gelmiş olabilecek yüksek öncelikli, etkin bir hizmet olayı. [Hizmet Durumu'na](https://portal.office.com/adminportal/home#/servicehealth)yönlendirerek herhangi bir danışma/olay olup olmadığını kontrol edin.
-   Sunucularda beklenmeyen olaylar nedeniyle meydana gelebilecek ve 30 dakikadan daha az süregelebilecek küçük bir otomatik iyileşme kurtarma senaryosu. 
    
    Bu küçük kurtarmalar için Mesaj Merkezi veya Hizmet Sağlık mesajları vardır ama çok yakında normale geri olmalıdır.

Çok az durumda, yukarıda listelenen üç senaryodan birinin neden olduğunu ve hizmetin geri yüklendiğini, ancak kullanıcıların tarayıcı önbelleğinin temizlenmediğini gözlemledik.

Lütfen siteye gitmeden önce tarayıcı önbelleğini temizlemeye çalış.

1. Microsoft Edge tarayıcınızda **Ayarlar'ı**seçin ve ardından **Gizlilik ve Güvenlik'i**seçin.
2. **Net tarama**altında, **neyi temizleyeceğini seç'i**seçin.
3. **Çerezleri ve kaydedilmiş web sitesi verilerini**seçin ve **Temizle'yi**seçin.

>[!Note] 
> Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken bu adımlar farklı olabilir.

>[!Note] 
> Başka bir seçenek, SharePoint sitenizi veya OneDrive'ınızı yeni bir InPrivate penceresinde açmak olacaktır.