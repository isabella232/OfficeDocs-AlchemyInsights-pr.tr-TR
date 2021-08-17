---
title: Gelen kutusu kurallarında gerçekleştirilen olayları bulma
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882655"
---
# <a name="find-events-performed-on-inbox-rules"></a>Gelen kutusu kurallarında gerçekleştirilen olayları bulma

Gelen kutusu kuralları oluşturulduğunda, değiştirdiğinde veya silindiğinde olaylar denetim günlüğüne kaydedilir. Bunları şu şekilde gözden geçirersiniz:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm **Denetimi'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim 'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

    > [!NOTE]
    > Denetimi açmamız gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.

2. Denetim **sayfasının** Ara **sekmesinde** aşağıdaki ayarları yapılandırabilirsiniz:
   - **Tarih ve saat aralığı:** Başlangıç ve Bitiş  kutularında **tarih/saat** aralığını seçin.
   - **Etkinlikler:** Select **New-InboxRule Create Inbox rule from Outlook Web App**

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Ayrıntılar açılır öğesini açmak için sonuçlardan bir etkinlik seçin. Parametreler **bölümünün** altında, kuralın adını, koşullar kümesi ve kuralın gerçekleştirecek eylemleri görebilirler.

Daha fazla bilgi edinmek için [bkz. Sık karşılaşılan destek sorunlarını araştırmak için denetim günlüğünde arama.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
