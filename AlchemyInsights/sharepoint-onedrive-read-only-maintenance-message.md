---
title: SharePoint veya OneDrive 'ı kullanmaya çalışırken bakım iletisi için salt okunur
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670852"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint veya OneDrive 'ı kullanmaya çalışırken bakım iletisi için salt okunur

Kullanıcılar, aşağıdaki senaryolardan biri için SharePoint veya OneDrive 'ı kullanmaya çalışırken **yalnızca bir salt okunur** ileti alabilir. 

-   Planlanmış veya etkin bir bakım etkinliği.  [Ileti merkezine](https://portal.office.com/adminportal/home#/messagecenter)giderek bunları denetleyin.
-   Yüksek öncelikli, etkin bir hizmet olayı olabilir. [Hizmet durumu](https://portal.office.com/adminportal/home#/servicehealth)'na giderek Danışma belgelerini/olaylarını denetleyin.
-   Sunucularda en çok 30 dak veya bu nedenle en son olabilecek beklenmeyen etkinlikler nedeniyle oluşabilecek küçük bir otomatik düzeltme Kurtarma senaryosu. 
    
    Bu küçük kurtarmalar için Ileti merkezi veya hizmet durumu gönderileri yok, ancak yine de normal çok yakında geri dönebilirsiniz.

Çok az, yukarıda listelenen üç senaryodan birinin neden olduğunu ve hizmet geri yüklendiğini gözlemlüyoruz, ancak kullanıcılar tarayıcı önbelleği temizlenmemiştir.

Lütfen siteye gitmeden önce tarayıcı önbelleğini temizlemeyi deneyin.

1. Microsoft Edge tarayıcınızda **Ayarlar**'ı seçin ve **Gizlilik ve güvenlik**'i seçin.
2. **Gezinmeyi temizle**altında, **neyin temizlensin 'i**seçin.
3. **Tanımlama bilgileri ve kaydedilmiş Web sitesi verilerini**seçip **Temizle**'yi seçin.

>[!Note] 
> Bu adımlar Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken farklılık gösterebilir.

>[!Note] 
> Başka bir seçenek de SharePoint sitenizi veya OneDrive 'ı yeni bir InPrivate penceresinde açar.