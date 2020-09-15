---
title: Denetim günlüklerindeki posta kutularındaki dış e-posta iletmeyi tanımlama
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696317"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Posta kutularında dış e-posta iletme 'nin ne zaman yapılandırıldığını belirleme

Bir Microsoft 365 kullanıcısı posta kutusunda dış e-posta iletmeyi yapılandırırsa, etkinlik, **Set-Mailbox** cmdlet 'inin bir parçası olarak denetlenir. Güvenlik & Uyumluluk Merkezi 'nde denetim günlüğü aramasını kullanarak etkinliği görebilirsiniz.

1. [Microsoft 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)'nde oturum açın.

2. **Search**  >  **Denetim günlüğü aramasını** ara sayfasına gidin.

3. **Başlangıç tarihi** ve **bitiş tarihi** alanlarında tarih aralığını seçin. Kullanıcı adı belirtmeniz gerekmez. **Etkinlikler** alanının **tüm etkinlikler için sonuçları gösterecek**şekilde ayarlandığını doğrulayın.

4. **Ara**'ya tıklayın.

Sonuçlarda, **Sonuçları filtrele** 'ye tıklayın ve etkinlik filtresi kutusuna **Set-Mailbox** yazın. Sonuçlarda bir denetim kaydı seçin. **Ayrıntılar** açılır listesinde, **ek bilgi**'yi tıklatın. Etkinliğin e-posta iletme ile ilgili olup olmadığını belirlemek için her bir denetim kaydının ayrıntılarına bakmanız gerekir.

- **ObjectID**: değiştirilmiş olan posta kutusunun diğer ad değeri.

- **Parametreler**: _ForwardingSMTPAddress_ hedef e-posta adresini gösterir.

- **Kullanıcı kimliği**: **ObjectID** alanındaki posta kutusunda e-postayı ileten Kullanıcı.

Daha fazla bilgi için, [posta kutusu için e-posta iletmeyi kimlerin görebileceğini belirleme](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)konusuna bakın.
