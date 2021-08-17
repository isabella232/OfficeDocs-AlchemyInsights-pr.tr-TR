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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895199"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Posta kutusunda iletmeyi ayarlayanları ve nasıl ayar olduğunu bulma

Posta kutusunda dış iletme ayarlanmışsa, Etkinlik **Set-Mailbox cmdlet'inin bir parçası** olarak denetlenebilir. Denetim günlüğünde etkinliği şu şekilde bulabilirsiniz:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm **Denetimi'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim 'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

   > [!NOTE]
   > Denetimi açmamız gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.

2. Denetim **sayfasında,** Arama sekmesinin **seçili olduğunu** doğrulayın ve sonra aşağıdaki ayarları yapılandırabilirsiniz:
   - Başlangıç ve Bitiş kutularında **tarih/saat** **aralığını** seçin.
   - Tüm etkinlikler **için sonuçları** **göster'i içeren Etkinlikler kutusunu doğrulayın.**

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Sonuçlarda, sonuçları **sıralamak için** Etkinlik sütununa tıklayın ve Posta **Kutusu girdilerini** ayarlayın.

5. Ayrıntılar açılır öğesini açmak için sonuçlardan bir etkinlik seçin. Etkinliğin e-posta iletmeyle ilgili olup olmadığını belirlemek için, her denetim kaydının ayrıntılarına bakabilirsiniz:
   - **ObjectId:** Değiştirilen posta kutusunun diğer ad değeri.
   - **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.
   - **UserId:** ObjectId alanında posta kutusunda e-posta iletmeyi **yapılandıran** kullanıcı.

Daha fazla bilgi için [bkz. Posta kutusu için e-posta iletmeyi kimlerin ayarlay olduğunu belirleme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
