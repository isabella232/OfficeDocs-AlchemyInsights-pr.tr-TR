---
title: Kiracı ilkesi (eylem geçersiz kılma) düzeltme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896095"
---
# <a name="fix-tenant-policy-action-override"></a>Kiracı ilkesi (eylem geçersiz kılma) düzeltme

İstenmeyen posta önleme ilkelerinizin biri bu iletiyi etkiliyordi. İlkeleri gözden geçirmek için aşağıdaki adımları izleyin:

1. aşağıdaki Microsoft 365 Defender portalında, İlkeler bölümünde <https://security.microsoft.com/> **E-posta &** İşbirliği \> **İlkeleri'&** Kurallar Tehdit ilkeleri \>  \> **İstenmeyen** postayla **mücadele'ye** gidin.

   Doğrudan İstenmeyen posta **önleme ilkeleri sayfasına gitmek** için, <https://security.microsoft.com/antispam> kullanın.

2. İstenmeyen posta önleme ilkeleri sayfasında, ilkenin adına tıklayarak ilkeyi  seçin (**Tür** Özel istenmeyen posta önleme ilkesi veya Ad, İstenmeyen posta önleme gelen  **ilkesidir (Varsayılan)**). 
3. Görüntülenen ayrıntılar açılır bölmesinde Eylemler bölümünde **Eylemleri düzenle'yi** seçin. 
4. İleti eylemleri **bölümünde,** aşağıdaki değerlerden herhangi biri seçili olup olmadığını  görmek için İstenmeyen Posta **,** Yüksek güven istenmeyen posta **,** Kimlik Avı ve Yüksek güven amaçlı kimlik avı kararlarını gözden geçirin:
   - **X üstbilgisi ekle**
   - **Konu satırına metin ekleme**
   - **İletiyi e-posta adresine yeniden yönlendirme**
   - **İletiyi silme**
   - **Eylem yok**

   Tüm müşterilere uygulanan **Standart ayarlar** iletiyi Exchange Online Protection iletiyi etkiliyor olabilir.

Daha fazla bilgi için [bkz. EOP'de istenmeyen posta önleme ilkelerini yapılandırma.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
