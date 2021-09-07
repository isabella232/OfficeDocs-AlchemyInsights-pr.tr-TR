---
title: EndPoint Manager - Güvenlik temelleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923574"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Güvenlik temelleri

Güvenlik temelleri, konuyla ilgili güvenlik ekipleri tarafından önerilen güvenlik ayarlarını uygulamaya yardımcı olmak üzere önceden yapılandırılmış Windows ayarı gruplarıdır. Bu temel gruplar yalnızca istenen ayarları ve değerleri sunacak şekilde özelleştirilebilir. Güvenlik temelleri hakkında daha fazla bilgi için bkz. [Intune’da Windows 10 cihazlarını yapılandırmak için güvenlik temellerini kullanma](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Şu anda aşağıdaki ürünler için güvenlik temelleri sağlanmıştır:

- Windows MDM Güvenlik ayarları
- Uç nokta için Microsoft Defender Güvenliği
- Microsoft Edge

Bu temellerden her biri düzenli aralıklarla güncelleştirilir ve artımlı sürümlerde kullanıma sunulur. Temelin güncel yönergelere uyduğundan emin olmak için her sürüm önce sürümlerin ayarlarına yenilerini ekler veya bazılarını kaldırır. Uç Nokta Güvenliği’ndeki Güvenlik temelleri konsolu bir sürümden diğerine yapılan değişiklikleri görünür hale getirerek farklı sürümlerin karşılaştırılmasına olanak tanır.

Güvenlik temelinin dağıtılacak olan sürümünü en etkili şekilde değiştirme yönergeleri için bkz. [Microsoft Intune’da güvenlik temeli profillerini yönetme](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Güvenlik temelini dağıttıktan sonra, dağıtımın durumunu izleyebilir ve tek tek cihazlara göre ayarları gözden geçirebilirsiniz.

Güvenlik taban çizgilerinin birçok ayarı olduğundan, tüm ayarların cihazlarınıza ve iş ihtiyaçlarına uygun olduğundan emin olmak için yapılandırma değişikliklerini gözden geçirmek ve test etmek önemlidir.

**Not:** Güvenlik temellerine ilişkin raporlama verilerinin görüntülenmesi, bir cihaza ilk dağıtım yapıldıktan sonra 24 saat kadar ve sonraki güncelleştirmelerde 6 saat kadar sürebilir. 

Temel ayarının uygulanmamasının en yaygın nedeni, aynı ayarın farklı bir profilde kullanılıyor olmasıdır. Belirli bir cihazda bu senaryoyu araştırmak için, Güvenlik Temeli profilinin Cihaz Durumu düğümünden söz konusu cihaz seçilebilir. Ayrıntılar için bkz. [Güvenlik temelleri için çakışmaları çözme](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).