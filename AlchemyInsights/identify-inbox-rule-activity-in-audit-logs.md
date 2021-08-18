---
title: Denetim günlüklerinde gelen kutusu kuralı etkinliğini belirleme
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331143"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Denetim günlüklerinde gelen kutusu kuralı etkinliğini belirleme

Gelen kutusu kuralı olaylarını (gelen kutusu kurallarını oluşturma, Microsoft 365 uyumluluk merkezi silme) görüntülemek için denetim günlüğü aramalarını kullanabilirsiniz.

1. Aşağıdaki adımlardan birini uygulayın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm Denetimi **'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - Aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

2. Denetim **sayfasının** Ara **sekmesinde** aşağıdaki ayarları yapılandırabilirsiniz:
   - **Tarih ve saat aralığı:** Başlangıç ve Bitiş  kutularında **tarih/saat** aralığını seçin.
   - **Etkinlikler:** Aşağıdaki değerlerden birini veya birden fazlasını seçin:
     - **Yeni Gelen KutusuSağdan gelen kutusu kuralı Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App.**
     - **Gelen kutusu kurallarını istemciden Outlook güncelleştirme**

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Ayrıntılar açılır öğesini açmak için sonuçlardan bir etkinlik seçin. Gelen kutusu kuralı ayarları hakkında bilgiler Parametreler **alanında** görüntülenir.

Daha fazla bilgi için [bkz. Kullanıcının bir gelen kutusu kuralı oluşturma olup olmadığını belirleme](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
