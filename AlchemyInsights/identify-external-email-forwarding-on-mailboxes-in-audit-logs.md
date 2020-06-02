---
title: Denetim günlüklerinde posta kutularında harici e-posta yönlendirmeyi tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508972"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Posta kutularında harici e-posta yönlendirmenin ne zaman yapılandırılma da olduğunu belirleme

Bir Microsoft 365 kullanıcısı bir posta kutusunda harici e-posta yönlendirmeyi yapılandırırsa, etkinlik **Set-Posta Kutusu** cmdlet'in bir parçası olarak denetlenir. Etkinliği Güvenlik & Uyumluluk Merkezi'nde denetim günlüğü aramasını kullanarak görebilirsiniz.

1. [Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/)oturum açın.

2. **Arama**  >  **Denetimi günlüğü arama** sayfasına gidin.

3. **Başlangıç tarihi** ve Bitiş **tarihi** alanlarındaki tarih aralığını seçin. Bir kullanıcı adı belirtmeniz gerekmez. **Etkinlikler** alanının tüm **etkinliklerin sonuçlarını gösterecek**şekilde ayarlı olduğunu doğrulayın.

4. **Arama'yı**tıklatın.

Sonuçlarda, **Sonuçları Filtrele'yi** ve etkinlik filtresi kutusunda **Set-Posta Kutusu** yazın'ı tıklatın. Sonuçlarda bir denetim kaydı seçin. **Ayrıntılar** flyout, **daha fazla bilgi**tıklatın. Etkinliğin e-posta yönlendirmeyle ilgili olup olmadığını belirlemek için her denetim kaydının ayrıntılarına bakmanız gerekir.

- **ObjectId**: Değiştirilen posta kutusunun diğer adı değeri.

- **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.

- **UserId**: **ObjectId** alanında posta kutusunda e-posta yönlendirmeyi yapılandıran kullanıcı.

Daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
