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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539121"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Dış e-posta iletme posta kutuları üzerinde yapılandırıldığında belirle

Office 365 kullanıcı posta kutusu bulunan dış e-posta iletme yapılandırır, etkinlik **Kümesi-posta kutusu** cmdlet'i bir parçası olarak denetlenir. Güvenlik & Uyumluluk Merkezi Denetim günlüğü aramayı kullanarak etkinliğini görebilirsiniz.

1. [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)oturum açın.

2. **Arama**gidin > **Denetim günlüğü arama** sayfası.

3. **Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin. Bir kullanıcı adı belirtmeniz gerekmez. **Tüm etkinlikler için sonuçları göstermek**için **etkinlikler** alanı olarak doğrulayın.

4. **Ara**' yı tıklatın.

Sonuçları **Filtre sonuçları** ' nı tıklatın ve **Set-posta kutusu** etkinlik filtre kutusunda yazın. Sonuçları bir denetim kaydı seçin. **Daha fazla bilgi** **Ayrıntılar** çıkma içinde tıklatın. Etkinlik iletme ilişkili olup olmadığını belirlemek için her bir denetim kaydı ayrıntılara bakmak zorunda.

- **NesneKimliği**: diğer ad değeri değiştirilmiş olan posta kutusu.

- **Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.

- **Kullanıcı kimliği**: **NesneKimliği** alanında posta kutusu e-posta iletme yapılandırılmış kullanıcı.

Daha fazla bilgi için bkz: [belirleme kimin e-posta iletmek için bir posta kutusu ayarlayın](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
