---
title: Denetim günlüklerini sil iletisi olayları tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539229"
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
