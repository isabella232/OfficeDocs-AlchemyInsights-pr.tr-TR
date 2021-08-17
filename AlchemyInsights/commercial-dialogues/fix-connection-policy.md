---
title: Bağlantı ilkesi düzeltme
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314864"
---
# <a name="fix-connection-policy"></a>Bağlantı ilkesi düzeltme

E-posta güvenli olarak işaretlendi ve kullanıcının Gelen Kutusu'na teslim edildi çünkü kaynak IP adresi varsayılan bağlantı filtresi ilkesinde güvenli olarak işaretlendi. İlkeyi gözden geçirmek için aşağıdaki adımları izleyin:

1. aşağıdaki Microsoft 365 Defender portalında, İlkeler bölümünde <https://security.microsoft.com/> **E-&** İşbirliği \> **İlkeleri'&** Kurallar Tehdit \>  \> **İlkeleri İstenmeyen** postayla **mücadele'ye** gidin.

   Doğrudan İstenmeyen posta **önleme ilkeleri sayfasına gitmek** için, <https://security.microsoft.com/antispam> kullanın.

2. **İstenmeyen posta önleme ilkeleri** sayfasında, ilkenin adına tıklayarak Bağlantı filtresi ilkesi **(Varsayılan)** adlı ilkeyi seçin.

3. Görüntülenen ayrıntılar açılır bölmesinde, Bağlantı filtreleme **bölümündeki Bağlantı filtresi ilkesi düzenle'ye** tıklayın. 

4. Her zaman aşağıdaki **IP** adreslerinden veya adres aralığından gelen iletilere izin ver bölümündeki girdileri gözden geçirin ve Güvenli listeyi **aç'ın seçili olupsına** bakın.

   **Not:** Microsoft, üçüncü taraf güvenilir gönderenlerin kaynaklarına abonedir. Güvenli liste etkinleştirilirse, bu güvenilir gönderenler yanlışlıkla istenmeyen posta olarak işaretlenir. Bu seçeneği öneririz, çünkü size gelen hatalı pozitif sonuç sayısını (istenmeyen posta olarak sınıflandırılmış iyi posta) azaltır.

Daha fazla bilgi için [bkz. Bağlantı filtrelemeyi yapılandırma.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
