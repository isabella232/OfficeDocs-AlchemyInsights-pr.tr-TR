---
title: Denetim günlüklerinde ileti silme olaylarını belirleme
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115668"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Silinmiş e-posta iletileri için denetim günlükleri

Ocak 2019'dan başlayarak, Microsoft posta kutusu denetim günlüğünü varsayılan olarak etkinleştirdi. Aksi takdirde, belirli bir kullanıcının ileti silme olaylarını gözden geçirmek için, denetlemeye yönelik silme eylemlerini el ile etkinleştirmeniz gerekir. Posta kutusu denetim günlüğü, sizin için veya belirli bir kullanıcı için zaten etkinleştirilmişse, aşağıdaki adımları izleyin.

1. [Uyumluluk Merkezi'Microsoft 365 oturum açma](https://protection.office.com/)

2. Arama **ve Araştırma'ya tıklayın** ve Denetim Günlüğü **Araması'yı seçin.**

3. Başlangıç tarihi ve Bitiş **tarihi alanlarında tarih** **aralığını** seçin. Araştırma yapmak istediğiniz kullanıcının kullanıcı adını belirtin (öğeleri silen kullanıcı). Etkinlikler alanında **Silinmiş öğeler** klasöründen silinmiş iletiler **ve İletiler Silinmiş** Öğeler **klasörüne taşındı öğesini seçin.**

4. **Arama'ya tıklayın.**

Sonuçlarda, bir denetim kaydı seçin. Ayrıntılar uç bilgisinde, Daha Fazla **Bilgi'ye tıklayın.** Silinen öğe hakkında ek bilgiler (örneğin, konu satırı ve silindiğinde öğenin konumu) **AffectedItems alanında** görüntülenir. **ClientInfoString özelliği,** silme işleminin Outlook, Web üzerinde Outlook (eski adı Outlook Web App) veya başka bir cihazda olup olduğunu gösterir.

Daha fazla bilgi için [bkz. Posta kutusu için e-posta iletmeyi kimlerin ayarlay olduğunu belirleme.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Not:** Silinmiş öğeleri denetim günlüğü özelliğini kullanarak geri alamayacak. Bir dosyadaki silinmiş iletileri Web üzerinde Outlook için [bkz.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)Outlook Web App.
