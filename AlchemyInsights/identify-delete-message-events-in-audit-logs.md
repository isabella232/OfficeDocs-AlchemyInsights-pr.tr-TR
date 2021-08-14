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
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868438"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Silinmiş e-posta iletileri için denetim günlükleri

Ocak 2019'dan başlayarak, Microsoft posta kutusu denetim günlüğünü varsayılan olarak etkinleştirdi. Aksi takdirde, belirli bir kullanıcının ileti silme olaylarını gözden geçirmek için, denetlemeye yönelik silme eylemlerini el ile etkinleştirmeniz gerekir. Posta kutusu denetim günlüğü, sizin için veya belirli bir kullanıcı için zaten etkinleştirilmişse, aşağıdaki adımları izleyin.

1. [Uyumluluk Merkezi'Microsoft 365 oturum açma](https://protection.office.com/)

2. Arama **ve Araştırma'ya tıklayın** ve Denetim Günlüğü **Araması'yı seçin.**

3. Başlangıç tarihi ve Bitiş **tarihi alanlarında tarih** **aralığını** seçin. Araştırma yapmak istediğiniz kullanıcının kullanıcı adını belirtin (öğeleri silen kullanıcı). Etkinlikler alanında **Silinmiş öğeler** klasöründen silinmiş iletiler **ve İletiler Silinmiş** Öğeler **klasörüne taşındı öğesini seçin.**

4. **Arama'ya tıklayın.**

Sonuçlarda, bir denetim kaydı seçin. Ayrıntılar uç bilgisinde, Daha Fazla **Bilgi'ye tıklayın.** Silinen öğe hakkında ek bilgiler (örneğin, konu satırı ve silindiğinde öğenin konumu) **AffectedItems alanında** görüntülenir. **ClientInfoString özelliği,** silme işleminin Outlook, Web üzerinde Outlook (eski adı Outlook Web App) veya başka bir cihazda olup olduğunu gösterir.

Daha fazla bilgi için [bkz. Posta kutusu için e-posta iletmeyi kimlerin ayarlay olduğunu belirleme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Not:** Silinmiş öğeleri denetim günlüğü özelliğini kullanarak geri alamayacak. Bir dosyadaki silinmiş iletileri Web üzerinde Outlook için [bkz. Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
