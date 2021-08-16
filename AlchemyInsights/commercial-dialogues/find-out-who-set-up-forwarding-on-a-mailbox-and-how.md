---
title: Posta kutusunda iletmeyi ayarlayanları ve nasıl ayar olduğunu bulma
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988253"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Posta kutusunda iletmeyi ayarlayanları ve nasıl ayar olduğunu bulma

Posta kutusunda dış iletme ayarlanmışsa, etkinlik bu cmdlet'in bir parçası Set-Mailbox denetlenr. Denetim günlüğünde etkinliği şu şekilde bulabilirsiniz:

1. Güvenlik ve [Uyumluluk Office 365 & gidin.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Arama **Denetimi günlüğü** araması öğesini >  **seçin.**
    > [!NOTE]
    > Denetimi açmamız gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.
1. Etkinlikler alanı, **Tüm etkinlikler** için sonuçları göster **(varsayılan) olarak ayarlanmış** olduğundan emin olun. Tarih aralığını belirtin. Kullanıcı adı belirtmenize gerek yok.
1. **Arama'ya seçin.** Etkinlikler Sonuçlar altında **görüntülenir.**
1. Sonuçları **Filtrele'yi** seçin ve **Ardından Etkinlik filtresi alanına Set-mailbox** girin.  Bu, tüm **Posta Kutusu Kümesi etkinliklerini** döndürür.
1. Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla Bilgi **öğesini seçin.** **Parametreler'in** altında, posta kutusunda ayarlanmış olan iletme e-posta adresini görebilirler. **UserID,** posta kutusunda dış iletmeyi ayarlaan kullanıcıyı temsil eder.
Daha fazla bilgi edinmek için [bkz. Sık Office 365 sorunlarını gidermek için denetim günlüğünde arama.](https://go.microsoft.com/fwlink/?linkid=2103944)