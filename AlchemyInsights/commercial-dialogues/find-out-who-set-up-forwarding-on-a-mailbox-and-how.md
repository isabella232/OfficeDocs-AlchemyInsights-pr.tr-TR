---
title: Posta kutusunda kimlerin iletmeyi ayarlay olduğunu ve nasıl ayar olduğunu bulma
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317828"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Posta kutusunda kimlerin iletmeyi ayarlay olduğunu ve nasıl ayar olduğunu bulma

Posta kutusunda dış iletme ayarlanmışsa, Etkinlik **Set-Mailbox cmdlet'inin bir parçası** olarak denetlenebilir. Denetim günlüğünde etkinliği şu şekilde bulabilirsiniz:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm Denetimi **'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - Aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

   **Not:** Denetimi açması gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.

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
