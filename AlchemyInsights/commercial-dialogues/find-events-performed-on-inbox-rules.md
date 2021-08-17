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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313519"
---
# <a name="find-events-performed-on-inbox-rules"></a>Gelen kutusu kurallarında gerçekleştirilen olayları bulma

Gelen kutusu kuralları oluşturulduğunda, değiştirdiğinde veya silindiğinde olaylar denetim günlüğüne kaydedilir. Bunları şu şekilde gözden geçirersiniz:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm Denetimi **'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - Aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

    **Not:** Denetimi açması gereken bir bildirim görüyorsanız, devam edin ve hemen açmayın. Bu özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.
1. Etkinlikler alanını seçin ve posta kutusu etkinliklerini Exchange bulun ve ardından Posta kutusu etkinliklerini New-InboxRule Kutusundan gelen kutusu kuralı oluştur'Outlook Web App. Bitirinca, Etkinlikler bölmesini simge durumuna küçültmek için bölmenin dışına tıklayın.
1. Tarih aralığını belirtin ve Kullanıcılar alanında, araştırma yapmak istediğiniz kullanıcının kullanıcı adını seçin. Bir defada birden çok kullanıcı seçin.
1. Ara'ya seçin. Etkinlikler Sonuçlar altında görünür.
1. Ayrıntıları görüntülemek için bir etkinlik seçin ve ardından Daha Fazla Bilgi'yi seçin. Parametreler bölümünün altında, kuralın adını, koşullar kümesi ve kuralın gerçekleştirecek eylemleri görebilirler.

2. Denetim **sayfasının** Ara **sekmesinde** aşağıdaki ayarları yapılandırabilirsiniz:
   - **Tarih ve saat aralığı:** Başlangıç ve Bitiş  kutularında **tarih/saat** aralığını seçin.
   - **Etkinlikler:** Select **New-InboxRule Create inbox rule from Outlook Web App**

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Ayrıntılar açılır öğesini açmak için sonuçlardan bir etkinlik seçin. Parametreler **bölümünün** altında, kuralın adını, koşullar kümesi ve kuralın gerçekleştirecek eylemleri görebilirler.

Daha fazla bilgi edinmek için [bkz. Sık karşılaşılan destek sorunlarını araştırmak için denetim günlüğünde arama.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
