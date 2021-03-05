---
title: İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482907"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor

**İşGünü'nde AD Kullanıcı Hazırlama karantina durumuna gidiyor ve AD'de hiçbir kullanıcı oluşturulamıyor**

İşGünü'nde AD Kullanıcı Hazırlama işi karantina durumuna geldi ve denetim günlükleri hata iletisiyle dışarı aktarma hatası olaylarını **gösteriyor: OperationsError-SvcErr: İşlem hatası oluştu. Dizin hizmeti için üstün başvuru yapılandırılmamış. Bu nedenle dizin hizmeti, bu ormanın dışındaki nesnelere başvuru yapamaz.** Bu hata genellikle Active Directory Kapsayıcı OU'su doğru ayarlanmamışsa veya **parentDistinguishedName** için kullanılan İfade Eşlemesinde sorun varsa ortaya konur.

Yazım hataları için Yeni Kullanıcılar için **Varsayılan** OU parametresini kontrol edin. Belirtilen OU'nun AD'nizin içinde zaten var olduğundan emin olun. Öznitelik eşlemesinde **parentDistinguishedName** kullanıyorsanız, her zaman AD etki alanı içinde bilinen bir kapsayıcıyı değerlendirdiğinden emin olun. Oluşturulan değeri görmek için denetim günlüklerinde Dışarı Aktar olayına bakın.

Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

