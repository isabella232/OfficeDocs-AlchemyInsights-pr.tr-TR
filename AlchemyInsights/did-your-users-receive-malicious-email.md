---
title: Kullanıcılarınız kötü amaçlı e-posta mı aldı?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326730"
---
# <a name="did-your-users-receive-malicious-email"></a>Kullanıcılarınız kötü amaçlı e-posta mı aldı?

Artık portalda Gönderiler'i kullanarak kötü amaçlı [e-postaları Microsoft'Microsoft 365 Defender bildirebilirsiniz.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Yönetici gönderimleri içinde [gönderilen iletiler](https://security.microsoft.com/reportsubmission?viewid=admin) taranır ve ayrıntılı çıkışta aşağıdaki sonuçlar görüntülenir:

- Teslim sırasında gönderenin e-posta kimlik doğrulamasında hata olup olmadığı.
- İletiyle ilgili kararı etkilemiş veya geçersiz kılmış olabilecek bir ilke eşleşmesi hakkında bilgi.
- İletide yer alan URL’lerin veya dosyaların kötü amaçlı olup olmadığını görmek için geçerli etkisizleştirme sonuçları.
- Derecelendirme yapanların geri bildirimi

Geçersiz kılma bulunursa, yeniden tarama işlemi birkaç dakika içinde tamamlanır. E-posta kimlik doğrulamasında sorun yoksa veya teslim bir geçersiz kılmadan etkilenmemişse, derecelendirme yapanların geri bildirimi bir gün kadar sürebilir.

İleti, URL veya dosyayla ilgili son karara (engellenme - engellenmeme kararı) katılmıyorsanız, yeniden taranması için bir gün sonra iletiyi tekrar gönderin. İleti yeniden gönderildikten sonra kararın değiştirilme olasılığı yüksektir.

Bu arada, [bu makalede](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) sağlanan yönergeleri izleyerek kötü amaçlı e-postayı kullanıcı gelen kutularından kaldırabilirsiniz.

- Office 365 için Microsoft Defender kullanan müşteriler:
  - Şüpheli [e-postaları bulmak ve silmek için Tehdit Gezgini'ni kullanma](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - Kötü amaçlı Kasa BIR [URL'ye erişimi engellemek için Hızlı](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) Bağlantılar'a tıklayın
  - Kötü amaçlı URL'lere tık kullanan ve erişilen kullanıcıları izleme: Kimlik avı URL'sini [görüntüle ve](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)karar verisi  &  [Al-UrlTrace'e tıklayın](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Otomatik [Araştırmayı el ile başlatma](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Ayrıca kötü amaçlı dosyalar ve URL’lerden korunmak için [Kötü amaçlı URL’ler ve dosyalardan koruma](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) adresinde sağlanan yönergeleri de izleyebilirsiniz.
