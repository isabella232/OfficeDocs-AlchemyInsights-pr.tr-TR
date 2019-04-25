---
title: Denetim günlüklerini sil iletisi olayları tanımlama
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416729"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Denetim günlükleri silinmiş e-posta iletileri için

Ocak 2019 içinde başlayarak, posta kutusu denetim günlüğü varsayılan olarak Microsoft açmak. Aksi halde, belirli bir kullanıcı için silme iletisi olayları gözden geçirmek için silme eylemleri denetleme için el ile etkinleştirmeniz gerekir. Posta kutusu denetim günlüğü zaten, kuruluşunuz için veya belirli bir kullanıcı için etkin, aşağıdaki adımları izleyin.

1. Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)

2. **Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.

3. **Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin. (Silinmiş öğeleri kullanıcı) incelemek istediğiniz kullanıcının kullanıcı adını belirtin. **Silinmiş Öğeler klasöründen silinen iletiler** ve **Silinmiş Öğeler klasörüne Moved iletiler** **Aktiviteler** alanında seçin.

4. **Ara**' yı tıklatın.

Sonuçlarda bir denetim kaydı seçin. Ayrıntılar çıkma **Daha fazla Bilgi'yi**tıklatın. Silinmiş bir öğeyi (örneğin, konu satırı ve onu silindiğinde öğenin konumunu) hakkında ek bilgi **AffectedItems** alanında görüntülenir. **ClientInfoString** özelliği, Outlook, Outlook web (eski adı Outlook Web App bilinir) veya başka bir aygıt silme işlemi oluştu, gösterecektir.

Daha fazla bilgi için bkz: [belirleme kimin e-posta iletmek için bir posta kutusu ayarlayın](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Not**: denetim günlüğü özelliğini kullanarak silinmiş öğeleri geri alamazsınız. Outlook Web silinmiş iletileri almak için bkz: [Recover silinmiş öğeleri Outlook Web App'te](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
