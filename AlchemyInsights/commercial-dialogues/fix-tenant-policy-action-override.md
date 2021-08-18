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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326817"
---
# <a name="fix-tenant-policy-action-override"></a>Kiracı ilkesi (eylem geçersiz kılma) düzeltme

İstenmeyen posta önleme ilkelerinizin biri bu iletiyi etkiliyordi. İlkeleri gözden geçirmek için aşağıdaki adımları izleyin:

1. aşağıdaki Microsoft 365 Defender portalında, İlkeler bölümünde <https://security.microsoft.com/> **E-&** İşbirliği \> **İlkeleri'&** Kurallar Tehdit \>  \> **İlkeleri İstenmeyen** postayla **mücadele'ye** gidin.

   Doğrudan İstenmeyen posta **önleme ilkeleri sayfasına gitmek** için, <https://security.microsoft.com/antispam> kullanın.

2. İstenmeyen posta önleme ilkeleri sayfasında, ilkenin adına tıklayarak ilkeyi  seçin (**Tür** Özel istenmeyen posta önleme ilkesi veya Ad, İstenmeyen posta önleme gelen  **ilkesidir (Varsayılan)**). 
3. Görüntülenen ayrıntılar açılır bölmesinde Eylemler bölümünde **Eylemleri düzenle'yi** seçin. 
4. İleti eylemleri **bölümünde,** aşağıdaki değerlerden herhangi biri seçili olup olmadığını  görmek için İstenmeyen Posta **,** Yüksek güven istenmeyen posta **,** Kimlik Avı ve Yüksek güven amaçlı kimlik avı kararlarını gözden geçirin:
   - **X üstbilgisi ekle**
   - **Konu satırına metin ekleme**
   - **İletiyi e-posta adresine yeniden yönlendirme**
   - **İletiyi silme**
   - **Eylem yok**

   Tüm müşterilere uygulanan **Standart ayarlar** iletiyi Exchange Online Protection etkilemektedir.

Daha fazla bilgi için [bkz. EOP'de istenmeyen posta önleme ilkelerini yapılandırma.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
