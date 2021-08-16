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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028776"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Posta kutularda dış e-posta iletmenin ne zaman yapılandırıldığından emin olun

Bir posta Microsoft 365 kullanıcı dış e-posta iletmeyi yapılandırıyorsa, etkinlik **Set-Mailbox cmdlet'i kapsamında** denetlenmektedir. Etkinlik, Güvenlik ve Uyumluluk Merkezi'nde denetim günlüğü arama &.

1. [Uyumluluk Merkezi'Microsoft 365 oturum açma.](https://protection.office.com/)

2. Arama Denetimi **günlüğü**  >  **araması sayfasına** gidin.

3. Başlangıç tarihi ve Bitiş **tarihi alanlarında tarih** **aralığını** seçin. Kullanıcı adı belirtmenize gerek yok. Etkinlikler **alanının Tüm** etkinlikler için sonuçları **göster olarak ayar olduğunu doğrulayın.**

4. **Arama'ya tıklayın.**

Sonuçlarda, Sonuçları **Filtrele'ye** tıklayın ve **etkinlik filtresi kutusuna Set-Mailbox** yazın. Sonuçlarda bir denetim kaydı seçin. Ayrıntılar uç **bilgisinde,** Daha fazla **bilgi'ye tıklayın.** Etkinliğin e-posta iletmeyle ilgili olup olmadığını belirlemek için, her denetim kaydının ayrıntılarına bakabilirsiniz.

- **ObjectId:** Değiştirilen posta kutusunun diğer ad değeri.

- **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.

- **UserId:** ObjectId alanında posta kutusunda e-posta iletmeyi **yapılandıran** kullanıcı.

Daha fazla bilgi için [bkz. Posta kutusu için e-posta iletmeyi kimlerin ayarlay olduğunu belirleme.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
