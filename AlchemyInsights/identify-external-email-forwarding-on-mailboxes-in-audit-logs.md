---
title: Denetim günlüklerinde posta kutularında dış e-posta iletmeyi belirleme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331179"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Posta kutularda dış e-posta iletmenin ne zaman yapılandırıldığından emin olun

Bir kullanıcı Microsoft 365 posta kutusunda dış e-posta iletmeyi yapılandırıyorsa, etkinlik **Set-Mailbox cmdlet'i kapsamında** denetlenmektedir. Denetim günlüğü aramalarını kullanarak etkinliği görüyoruz. Bunu nasıl yapacağım?

1. Aşağıdaki adımlardan birini uygulayın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm Denetimi **'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - Aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://sip.security.microsoft.com/auditlogsearch> kullanın.

2. Denetim **sayfasında,** Arama sekmesinin **seçili olduğunu** doğrulayın ve sonra aşağıdaki ayarları yapılandırabilirsiniz:
   - Başlangıç ve Bitiş kutularında **tarih/saat** **aralığını** seçin.
   - Tüm etkinlikler **için sonuçları** **göster'i içeren Etkinlikler kutusunu doğrulayın.**

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Sonuçlarda, Sonuçları **Filtrele'ye** tıklayın ve **etkinlik filtresi kutusuna Set-Mailbox** yazın.

5. Sonuçlarda bir denetim kaydı seçin. Ayrıntılar uç **bilgisinde,** Daha fazla **bilgi'ye tıklayın.** Etkinliğin e-posta iletmeyle ilgili olup olmadığını belirlemek için, her denetim kaydının ayrıntılarına bakabilirsiniz.

   - **ObjectId:** Değiştirilen posta kutusunun diğer ad değeri.
   - **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.
   - **UserId:** ObjectId alanında posta kutusunda e-posta iletmeyi **yapılandıran** kullanıcı.

Daha fazla bilgi için [bkz. Posta kutusu için e-posta iletmeyi kimlerin ayarlay olduğunu belirleme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
