---
title: Linux'ta Uç Nokta için Microsoft Defender performans sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794223"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Linux'ta Uç Nokta için Microsoft Defender performans sorunları

Bu makale, Linux'ta Uç Nokta için Microsoft Defender performans sorunlarını belirleme adımsında size yol sunar.

Öncelikle, en son sürümle karşılaşan sorunun çözülmüş olduğunu [doğrulamanız önemlidir.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Araştırmanızı başlatmak için bkz. [Linux'ta Uç Nokta için Microsoft Defender performans sorunlarını giderme.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Dışlamalar

Dışlamalar performans sorunlarının azaltmak için yardımcı olabilir. Ek riskler bilindiği ve belgelenmiş olduğu için, başlamadan önce dışlamalarınızı gözden geçirebilirsiniz.

Daha fazla bilgi için [bkz. Linux'ta Uç Nokta için Microsoft Defender için dışlamaları yapılandırma ve doğrulama.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Dışlamak istediğiniz & çok dosya varsa ve hepsi aynı bağlama üzerinde olduğunda, bağlama klasörünü dışarıda tutmak daha kolay olabilir. Şubat sürümü 101.22.80'den başlayarak tüm mountpoint'i dahil çekesiniz.

Örneğin, /mnt/backup bir mountpoint ise, şu komutu çalıştırarak dışlama listesine /mnt/backup ekleyebilirsiniz:

`$ mdatp exclusion folder add –path /mnt/backup`

**Not:** Dışlamaların eklanması kötü amaçlı yazılım algılanma riskini artırır ve özenli bir şekilde ele geçiril olmalı ve uygulanmalı.

## <a name="need-help"></a>Yardıma mı ihtiyacınız var?

Size en verimli şekilde yardımcı olmak için bir destek durumu açmadan önce tanılama verilerini toplayın.
