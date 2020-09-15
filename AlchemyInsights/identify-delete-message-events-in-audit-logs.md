---
title: Denetim günlüklerinde ileti etkinliklerini silme
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696533"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Silinen e-posta iletilerinin günlüklerini denetleme

2019 Ocak tarihinde başlayarak varsayılan olarak posta kutusu denetim günlüğü açılıyor. Başka türlü, belirli bir kullanıcının ileti etkinliklerini gözden geçirmek için, denetim için silme eylemlerini el ile etkinleştirmeniz gerekir. Kuruluşunuz için posta kutusu denetim günlüğü zaten etkinleştirilmişse veya belirli bir kullanıcı için aşağıdaki adımları izleyin.

1. [Microsoft 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/) 'nde oturum açma

2. **Arama ve araştırma** 'ya tıklayın ve **Denetim günlüğü araması**'nı seçin.

3. **Başlangıç tarihi** ve **bitiş tarihi** alanlarında tarih aralığını seçin. Araştırmak istediğiniz kullanıcı için Kullanıcı adını belirtin (öğeleri silmiş olan Kullanıcı). **Etkinlikler** alanında, **Silinmiş Öğeler klasöründen silinmiş iletiler** 'ı seçin ve **iletileri Silinmiş Öğeler klasörüne taşındı**.

4. **Ara**'ya tıklayın.

Sonuçlarda bir denetim kaydı seçin. Ayrıntılar açılır listesinde, **ek bilgi**'yi tıklatın. Silinmiş öğe hakkındaki ek bilgileri (örneğin, konu satırı ve silindiğinde öğenin konumu) **AffectedItems** alanında görüntülenir. **Clıtinfostring** özelliği, silme işleminin Outlook, Web üzerinde Outlook (önceki adıyla Outlook Web App) veya başka bir cihazdan silinmesi durumunda gösterilir.

Daha fazla bilgi için, [posta kutusu için e-posta iletmeyi kimlerin görebileceğini belirleme](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)konusuna bakın.

**Not**: denetim günlüğü özelliğini kullanarak silinmiş öğeleri alamazsınız. Web üzerinde Outlook 'ta silinmiş iletileri almak için, [Outlook Web App 'te silinmiş öğeleri kurtarma](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)konusuna bakın.
