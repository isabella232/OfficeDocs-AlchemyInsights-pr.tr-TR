---
title: EndPoint Manager - Güvenlik taban çizgisi
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421218"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Güvenlik taban çizgisi

Güvenlik taban çizgisi, ilgili güvenlik ekipleri tarafından önerilen güvenlik ayarlarını uygulamanıza yardımcı olan önceden yapılandırılmış Windows ayarları gruplarıdır. Bu taban çizgisi, yalnızca istediğiniz ayarları ve değerleri sunmak için özelleştirilebilir. Güvenlik taban çizgisi hakkında daha fazla bilgi için Bkz. [Intune'da Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)cihazlarını yapılandırmak için güvenlik taban çizgilerini kullanma.

Şu anda bu ürünlerin taban çizgilerini vardır:

- Windows MDM Güvenlik ayarları
- EndPoint Güvenliği için Microsoft Defender
- Microsoft Edge

Taban çizgilerinin her biri düzenli olarak güncelleştirilir ve artımlı sürümlerde yayımlanır. Taban çizgisinin geçerli kılavuz çizgiye uygun olduğundan emin olmak için, her sürüm önceki sürümden ayarları ekler ve kaldırır. Uç Nokta Güvenliği'nin Güvenlik taban çizgisi konsolu, sürümden sürüme yapılan değişikliklerin görünür olmasıyla farklı sürümlerin karşılaştırmasına olanak sağlar.

Temelin hangi sürümünün dağıtılacağı konusunda yol gösterici bilgi için, Microsoft Intune'da güvenlik temeli [profillerini yönetme makalelerine bakın.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Güvenlik temelini dağıttırdikten sonra, dağıtım durumunu izleyebilir ve ayarları cihaz temelinde gözden geçirebilirsiniz.

**Not:** Taban çizgilerinin raporlama verileri, ilk dağıtımdan bir cihaza 24 saat ve daha sonraki güncelleştirmeler için 6 saate kadar sürebilir. 

Taban çizgisi ayarının uygulamamalarının en yaygın nedeni, aynı ayarın farklı bir profilde kullanılıyor olmasıdır. Bu senaryo, Belirli bir cihaz için, Güvenlik Temeli profilinin Cihaz Durumu düğümünden seçerek araştırabilirsiniz. Ayrıntılar için [bkz. Güvenlik taban çizgilerine ilişkin çakışmaları çözme.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)