---
title: Silinen olayların denetim günlüklerini okuma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483321"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Silinen olayların denetim günlüklerini okuma

Bunu şu şekilde yapacaksınız:

1. [Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Arama **Denetimi günlüğü** arama öğesini  >  [**seçin.**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > Özelliği açmak için ihtiyacınız olduğunu fark ediyorsanız, şimdi devam edin ve özelliği açabilirsiniz. Özellik açık değilse, arama sonuçları önceki tarihlerden veri alamı olmayacaktır.
1. **Etkinlikler'i** seçin ve **ardından Exchange posta kutusu etkinliklerini bulun.** Silinmiş Öğeler **klasöründeki Silinmiş iletiler ve** İletiler **Silinmiş Öğeler klasör seçeneklerine** taşındı seçeneklerini belirleyin. Bitir bittiğinde, Etkinlikler bölmesini simge durumuna küçültmek için **bölmenin dışına** tıklayın.
1. Tarih aralığını belirtin ve Kullanıcılar  kutusunda araştırma yapmak istediğiniz kullanıcının kullanıcı adını seçin. Bir defada birden çok kullanıcı seçin.
1. **Ara'ya seçin.** Etkinlikler Sonuçlar altında **görüntülenir.**
1. Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla **Bilgi'yi seçin.** Silinen öğe hakkında konu satırı ve silindiğinde öğenin konumu gibi ek bilgiler **AffectedItems alanında** görüntülenir.
    > [!NOTE]
    > Denetim günlüğü özelliğini kullanarak silinmiş öğeleri geri yükleyemezsiniz. Silinmiş öğeleri geri yüklemek için, Outlook [Web App'te silinmiş öğeleri veya e-postayı kurtarma'ya bakın.](https://go.microsoft.com/fwlink/?linkid=2103759)

Daha fazla bilgi edinmek için, sık karşılaşılan senaryoların sorunlarını gidermek için [Office 365 denetim günlüğünde aramama bakın.](https://go.microsoft.com/fwlink/?linkid=2103944)
