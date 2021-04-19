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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815266"
---
# <a name="did-your-users-receive-malicious-email"></a>Kullanıcılarınız kötü amaçlı e-posta mı aldı?

- Artık [Güvenlik ve Uyumluluk Merkezi’nde Yönetici Gönderimleri](https://sip.protection.office.com/reportsubmission)’ni kullanarak kötü amaçlı e-postayı Microsoft’a bildirebilirsiniz.

[Yönetici gönderimlerinde](https://sip.protection.office.com/reportsubmission) gönderdiğiniz iletiler taranır ve **ayrıntılar** açılır öğesinde aşağıdaki sonuçlar gösterilir:

- Teslim sırasında gönderenin e-posta kimlik doğrulamasında hata olup olmadığı.
- İletiyle ilgili kararı etkilemiş veya geçersiz kılmış olabilecek bir ilke eşleşmesi hakkında bilgi.
- İletide yer alan URL’lerin veya dosyaların kötü amaçlı olup olmadığını görmek için geçerli etkisizleştirme sonuçları.
- Derecelendirme yapanların geri bildirimi

Geçersiz kılma bulunursa, yeniden tarama işlemi birkaç dakika içinde tamamlanır. E-posta kimlik doğrulamasında sorun yoksa veya teslim bir geçersiz kılmadan etkilenmemişse, derecelendirme yapanların geri bildirimi bir gün kadar sürebilir.

İleti, URL veya dosyayla ilgili son karara (engellenme - engellenmeme kararı) katılmıyorsanız, yeniden taranması için bir gün sonra iletiyi tekrar gönderin. İleti yeniden gönderildikten sonra kararın değiştirilme olasılığı yüksektir.

Bu arada, [bu makalede](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) sağlanan yönergeleri izleyerek kötü amaçlı e-postayı kullanıcı gelen kutularından kaldırabilirsiniz.

- Office 365 için Microsoft Defender kullanan müşteriler:
    - [Şüpheli e-postayı bulmak ve silmek için Tehdit Gezgini’ni](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) kullanabilir
    - kötü amaçlı URL’ye [erişimi engellemek için Güvenli Bağlantıları kullanabilir](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)
    - kötü amaçlı URL’leri tıklayan ve bu URL’lere erişen kullanıcıları izleyebilir: [Kimlik avı URL’sini görüntüleme ve karar verilerine tıklama](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - el ile [Otomatik Araştırma başlatabilir](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Ayrıca kötü amaçlı dosyalar ve URL’lerden korunmak için [Kötü amaçlı URL’ler ve dosyalardan koruma](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) adresinde sağlanan yönergeleri de izleyebilirsiniz.