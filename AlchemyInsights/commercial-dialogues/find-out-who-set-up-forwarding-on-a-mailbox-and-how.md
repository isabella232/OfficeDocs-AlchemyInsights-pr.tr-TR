---
title: Posta kutusunda kimlerin iletmeyi ayarlay olduğunu ve nasıl olduğunu bulma
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483357"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Posta kutusunda kimlerin iletmeyi ayarlay hazır olduğunu ve nasıl olduğunu bulma

Posta kutusunda dış iletme ayarlanmışsa, etkinlik bir posta kutusu cmdlet'i Set-Mailbox denetlenr. Denetim günlüğünde etkinliği şu şekilde bulabilirsiniz:

1. [Office 365 Güvenlik ve Uyumluluk & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Arama **Denetimi günlüğü** arama öğesini >  **seçin.**
    > [!NOTE]
    > Denetimi açmamız gereken bir bildirim görüyorsanız, şimdi devam edin ve bu bildirimi açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri alamı olmayacaktır.
1. Etkinlikler **alanı, tüm etkinlikler** için sonuçları göster **(varsayılan) olarak** ayarlanmış olduğundan emin olun. Tarih aralığını belirtin. Kullanıcı adı belirtmenize gerek yok.
1. **Ara'ya seçin.** Etkinlikler Sonuçlar altında **görüntülenir.**
1. Sonuçları **Filtrele'yi** seçin ve ardından Etkinlik filtresi alanına **Set-mailbox** girin.  Bu, tüm **Posta Kutusu Kümesi etkinliklerini** döndürür.
1. Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla **Bilgi'yi seçin.** **Parametreler'in** altında, posta kutusunda ayarlanmış olan iletme e-posta adresini kullanabilirsiniz. **UserID,** posta kutusunda dış iletmeyi ayar eden kullanıcıyı temsil eder.
Daha fazla bilgi edinmek için, sık karşılaşılan senaryoların sorunlarını gidermek için [Office 365 denetim günlüğünde aramama bakın.](https://go.microsoft.com/fwlink/?linkid=2103944)