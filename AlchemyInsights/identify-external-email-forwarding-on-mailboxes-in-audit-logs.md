---
title: Dış e-posta İletim Denetim günlüklerini de posta kutuları belirle
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383117"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Dış e-posta iletme posta kutuları üzerinde yapılandırıldığında belirle

Bir kullanıcı bir posta kutusuna dış e-posta iletme yapılandırır, etkinlik **Kümesi-posta kutusu** cmdlet'i bir parçası olarak denetlenir. Güvenlik & Uyumluluk Merkezi Denetim günlüğü aramayı kullanarak etkinliğini görebilirsiniz.

1. Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)

2. **Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.

3. **Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin. Bir kullanıcı adı belirtmeniz gerekmez. **Tüm etkinlikler için sonuçları göstermek**için **etkinlikler** alanı olarak doğrulayın.

4. **Ara**' yı tıklatın.

Sonuçları **Filtre sonuçları** ' nı tıklatın ve **Set-posta kutusu** etkinlik filtre kutusunda yazın. Sonuçları bir denetim kaydı seçin. **Daha fazla bilgi** **Ayrıntılar** çıkma içinde tıklatın. Etkinlik iletme ilişkili olup olmadığını belirlemek için her bir denetim kaydı ayrıntılara bakmak zorunda.

- **NesneKimliği**: diğer ad değeri değiştirilmiş olan posta kutusu.

- **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.

- **Kullanıcı kimliği**: **NesneKimliği** alanında posta kutusu e-posta iletme yapılandırılmış kullanıcı.

Daha fazla bilgi için bkz: [belirleme kimin e-posta iletmek için bir posta kutusu ayarlayın](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
