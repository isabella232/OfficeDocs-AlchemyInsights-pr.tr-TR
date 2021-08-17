---
title: Denetim günlüğünde IP adresini bulma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303597"
---
# <a name="find-the-ip-address-in-audit-log"></a>Denetim günlüğünde IP adresini bulma

Kullanıcı veya yönetici tarafından gerçekleştirilen bir faaliyete karşılık gelen IP adresi denetim günlüklerinde gösterilir. Müşteri bilgileri de günlüğe kaydedilir. IP adresini şu şekilde tanımlayabilirsiniz:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm Denetimi **'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - Aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

    **Not:** Denetimi açması gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik etkin değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.

2. Denetim **sayfasında,** Arama sekmesinin **seçili olduğunu** doğrulayın ve sonra aşağıdaki ayarları yapılandırabilirsiniz:
   - **Tarih ve saat aralığı:** Başlangıç ve Bitiş  kutularında **tarih/saat** aralığını seçin.
   - **Etkinlikler:** Belirli bir etkinlikle ilgileniyorsanız, listeden seçin; aksi takdirde, tüm **etkinlikler için sonuçları göster varsayılan değeri** tüm etkinlikleri döndürür. Belirli etkinliklerin seçim için kullanılamıyor olabileceğini unutmayın; Bununla birlikte, Tüm etkinlikler için sonuçları **göster seçiliyse, bu denetim öğeleri** döndürülür.
   - **Kullanıcılar:** Tüm kullanıcıların sonuçlarını sonuç olarak almak için boş varsayılan değeri kabul etme veya bir veya birden çok kullanıcı girin.

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Sonuçlarda, Sonuçları **Filtrele'ye** tıklayın ve **etkinlik filtresi kutusuna Set-Mailbox** yazın.

5. Ayrıntılar açılır öğesini açmak için sonuçlarda bir **denetim kaydı** seçin.

Daha fazla bilgi için [bkz. Sık karşılaşılan destek sorunlarını araştırmak için denetim günlüğünde arama.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
