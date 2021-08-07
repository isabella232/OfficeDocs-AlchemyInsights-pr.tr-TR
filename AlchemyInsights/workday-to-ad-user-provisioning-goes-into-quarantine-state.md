---
title: İşgünü AD Kullanıcı Hazırlama karantina durumuna gidiyor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036512"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>İşgünü AD Kullanıcı Hazırlama karantina durumuna gidiyor

**Ad Kullanıcı Hazırlama iş günü karantina durumuna gidiyor ve AD'de hiçbir kullanıcı oluşturulamıyor**

AD Kullanıcı Sağlama işinin çalışma günü karantina durumuna getirildi ve denetim günlükleri **Hata: OperationsError-SvcErr: bir işlem hatası oluştu hata iletisini görüntüler. Dizin hizmeti için üstün başvuru yapılandırılmamış. Bu nedenle dizin hizmeti, bu ormanın dışındaki nesnelere başvuru ve yapamaz.** Bu hata, genellikle Active Directory Container OU doğru ayarlanmamışsa veya **parentDistinguishedName** için kullanılan İfade Eşlemesinde sorun varsa ortaya konur.

Yazım hataları için Yeni Kullanıcılar için **Varsayılan** OU parametresini kontrol edin. Belirtilen OU'nun AD'niz içinde zaten olduğundan emin olun. Öznitelik eşlemesinde **parentDistinguishedName** kullanıyorsanız, her zaman AD etki alanı içindeki bilinen bir kapsayıcıyı hesap olduğundan emin olun. Oluşturulan değeri görmek için denetim günlüklerinde Export olayına bakın.

Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için bkz. [Öğretici: Otomatik kullanıcı sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

