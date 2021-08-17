---
title: Silinen olayların denetim günlüklerini okuma
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896035"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Silinen olayların denetim günlüklerini okuma

Bunu şu şekilde yapacaksınız:

1. Aşağıdaki eylemlerden birini yapın:
   - Aşağıdaki Microsoft 365 uyumluluk merkezi , <https://compliance.microsoft.com> Çözüm **Denetimi'ne** \> **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://compliance.microsoft.com/auditlogsearch> kullanın.
   - aşağıdaki Microsoft 365 Defender portalında <https://security.microsoft.com> Denetim 'e **gidin.** Veya doğrudan Denetim sayfasına **gitmek için** <https://security.microsoft.com/auditlogsearch> kullanın.

    > [!NOTE]
    > Özelliği açman gerektir diye bir bildirim görüyorsanız, şimdi devam edin ve özelliği açabilirsiniz. Özellik açık değilse, arama sonuçları önceki tarihlerden veri çekebilirsiniz.

2. Denetim **sayfasının** Ara **sekmesinde** aşağıdaki ayarları yapılandırabilirsiniz:
   - **Tarih ve saat aralığı:** Başlangıç ve Bitiş  kutularında **tarih/saat** aralığını seçin.
   - **Etkinlikler:** Posta **Exchange etkinlikleri girin** ve ardından aşağıdaki değerleri seçin:
     - **Silinmiş Öğeler klasöründen silinmiş iletiler**
     - **İletiler Silinmiş Öğeler klasörüne taşındı**

       Bitirinca, Etkinlikler bölmesini simge durumuna küçültmek için bölmenin **dışına** tıklayın.

   - **Kullanıcılar:** Tüm kullanıcıların sonuçlarını sonuç olarak almak için boş varsayılan değeri kabul etme veya bir veya birden çok kullanıcı girin.

3. Bitirdikten sonra Ara'ya **tıklayın.** Etkinlikler, yeni Denetim arama **sayfasında** görüntülenir.

4. Ayrıntılar açılır öğesini açmak için sonuçlardan bir etkinlik seçin. Silinen öğe hakkında ek bilgiler, örneğin konu satırı ve silindiğinde öğenin konumu **AffectedItems alanında** görüntülenir.

   > [!NOTE]
   > Denetim günlüğü özelliğini kullanarak silinmiş öğeleri geri yüklemezsiniz. Silinmiş öğeleri geri yüklemek için [bkz. Bir dosyadaki silinmiş e-Web üzerinde Outlook.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Daha fazla bilgi için [bkz. Sık karşılaşılan destek sorunlarını araştırmak için denetim günlüğünde arama.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
