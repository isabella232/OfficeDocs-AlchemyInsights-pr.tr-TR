---
title: Read-Only veya bağlantı kullanmayı denerken Bakım SharePoint iletisinde OneDrive
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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329468"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only veya bağlantı kullanmayı denerken Bakım SharePoint iletisinde OneDrive

Kullanıcılar, aşağıdaki **senaryolardan biri için** Bakım için Salt SharePoint veya OneDrive İletisi alabilirsiniz. 

-   Planlanan veya etkin bir bakım etkinliği.  İleti Merkezi'ne giderek onları [kontrol edin.](https://portal.office.com/adminportal/home#/messagecenter)
-   Yüksek öncelikli, etkin bir hizmet olayı olabilir. Hizmet Durumu'na giderek herhangi bir tavsiyeyi/olayı [denetleme.](https://portal.office.com/adminportal/home#/servicehealth)
-   Sunucularda 30 dakikadan kısa bir süre devam ede postası olan beklenmeyen olayların nedeni çok küçük bir otomatik kurtarma senaryosu. 
    
    Bu küçük kurtarmalar için İleti Merkezi veya Hizmet Durumu gönderisi yoktur, ancak çok yakında normale dönersiniz.

Çok az durumda, yukarıda listelenen üç senaryodan birinin nedeni olduğunu ve hizmetin geri yüklendi ancak kullanıcıların tarayıcı önbelleğinin temizlenmemiş olduğunu gözlemlemektedir.

Siteye gitmeden önce lütfen tarayıcı önbelleğini temizlemeyi deneyin.

1. Microsoft Edge tarayıcınızda Ayarlar **ve** ardından Gizlilik ve Güvenlik **öğesini seçin.**
2. Gözatma **temizle altında,** **Temizlenecekleri seç öğesini seçin.**
3. Tanımlama bilgileri **ve kaydedilen web sitesi verileri'ne tıklayın** ve Temizle'ye **tıklayın.**

**Not:** Mozilla Firefox veya Google Chrome gibi diğer tarayıcıları kullanırken bu adımlar farklı olabilir.

**Not:** Bir diğer seçenek de SharePoint InPrivate penceresini açmak OneDrive dosyanızı açmaktır.