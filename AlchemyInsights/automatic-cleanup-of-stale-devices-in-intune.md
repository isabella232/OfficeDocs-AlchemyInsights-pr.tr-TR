---
title: Intune'da bayat cihazların otomatik olarak temizlenmesi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555737"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Intune'da bayat cihazların otomatik olarak temizlenmesi

Intune, yöneticinin 90 ile 270 gün arasında bir zaman aralığı yapılandırmasına olanak tanır ve bu süre den sonra eski aygıtlar hizmetten kaldırılır. Bu ayar kuruluş genelindedir ve etkinleştirildiğinde hemen yürürlüğe girer. Ayarı aşan bir süre için Intune sunucusunda denetlenen tüm aygıtlar kalıcı olarak silinir.

**Not** Bu temizleme eylemi için yalnızca MDM aygıt nesneleri uygundur. EAS yalnızca aygıt nesneleri hariç tutulur.

Bir aygıtın aygıt temizleme kurulumuna ve "durumuna" bağlı olarak silinme için ne zaman uygun hale gelmesi hakkında daha fazla bilgi için:

Ayar: **Son iade tarihinden sonra aygıtları silme: Evet (belirtilen günlerde bazı değer (N))**

- Ayarda yapılandırılan değer (N) değerine göre, Intune hizmeti aygıtı son başarıyla giriş yaptıktan sonraki gün içinde siler.

Ayar: **Son iade tarihinden sonra aygıtları silme: Hayır**

- Cihaz sertifikasının süresi dolduktan ve yenilenmedikten 180 gün sonra aygıt silinir.

**Not** Her iki durumda da, aygıtın Intune'da başarıyla kaydedilmesi gerekir. Kayıt, Intune hizmetiyle yapılan ilk cihaz denetimi sırasında gerçekleşir.

Bir aygıt Başarılı bir şekilde Intune'a kaydolursa ancak Intune kayıtlı değilse, aygıt kayıttan 270 gün sonra silinir. (Aygıtı iptal edilmiş olarak işaretlemek için 90 gün, kaydı silmek için ise 180 gün daha.)

Şu anda Intune konsolunda, belirli bir aygıt için aygıt sertifikasının son kullanma tarihini belirlemek için bir mekanizma bulunmamaktadır.