---
title: Read-Only veya bağlantı kullanmayı denerken Bakım SharePoint OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910566"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only veya bağlantı kullanmayı denerken Bakım SharePoint OneDrive

Kullanıcılar, aşağıdaki **senaryolardan biri için** Bakım için Salt SharePoint veya OneDrive İletisi alabilirsiniz. 

-   Planlanan veya etkin bir bakım etkinliği.  İleti Merkezi'ne giderek onları [kontrol edin.](https://portal.office.com/adminportal/home#/messagecenter)
-   Yüksek öncelikli, etkin bir hizmet olayı olabilir. Hizmet Durumu'na giderek herhangi bir tavsiyeyi/olayı [denetleme.](https://portal.office.com/adminportal/home#/servicehealth)
-   Sunucularda 30 dakikadan kısa bir süre devam ede beklenmeyen olayların nedeni olan küçük bir otomatik kurtarma senaryosu. 
    
    Bu küçük kurtarmalar için İleti Merkezi veya Hizmet Durumu gönderisi yoktur, ancak çok yakında normale dönersiniz.

Çok az sayıda durumda, yukarıda listelenen üç senaryodan birinin nedeni olduğunu ve hizmetin geri yüklendi ancak kullanıcıların tarayıcı önbelleğinin temizlenmemiş olduğunu gözlemle değildi.

Siteye gitmeden önce lütfen tarayıcı önbelleğini temizlemeyi deneyin.

1. Microsoft Edge tarayıcınızda Ayarlar **ve** ardından Gizlilik ve Güvenlik **öğesini seçin.**
2. Gözatma **temizle altında,** **Temizlenecekleri seç öğesini seçin.**
3. Tanımlama bilgileri **ve kaydedilen web sitesi verileri'ne tıklayın** ve Temizle'ye **tıklayın.**

>[!Note] 
> Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken bu adımlar farklılık gösterebilir.

>[!Note] 
> Bir diğer seçenek de SharePoint InPrivate penceresinde OneDrive dosyanızı açmak olabilir.