---
title: Windows için Microsoft Defender ile ilgili sık karşılaşılan sorunları Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330080"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Windows için Microsoft Defender ile ilgili sık karşılaşılan sorunları Office 365

Aşağıdakiler, Windows için Microsoft Defender ile ilgili yaygın sorunların bazı Office 365:

- **İleti gecikmesi:**

  E-posta teslimi gecikmeleri E-Kasa İletileri tarama eki nedeniyle olabilir. Daha fazla bilgi için [bkz. Kasa ilkesi ayarlarını değiştirme](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Hatalı pozitif veya negatif sonuçları bildirme**:

  Daha fazla bilgi için [bkz. İletileri ve dosyaları Microsoft'a bildirme](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Bağlantı Kasa korumasını etkinleştirme:**

  1. aşağıdaki Microsoft 365 Defender portalında, İlkeler bölümündeki & İşbirliği İlkeleri'ne & Tehdit <https://security.microsoft.com/>  \>  \>  \> **Kasa** **Bağlantılar'a** gidin.

     Doğrudan Bağlantılar sayfasına **Kasa için,** <https://security.microsoft.com/safelinksv2> kullanın.

  2. Yeni **Kasa sayfasında,** ilkenin adına tıklayarak ilkeyi seçin.
  3. Görüntülenen ayrıntılar açılır yapısında, aşağıdaki adımlardan birini uygulayın:
     - Yeni ilke eklemek için + Oluştur **öğesini seçin.** İlke ayarlarınızı tanımlamanıza yardımcı olacak bir sihirbaz başlatır.
     - Var olan bir ilkeyi düzenlemek için, ilkenin adına tıklayarak ilkeyi seçin. Görüntülenen ayrıntılar açılır sayfasında, Koruma ayarları **bölümünde** **Düzenle'yi** seçin.
  4. Koruma **ayarları sayfasında** aşağıdaki ayarları yapılandırabilirsiniz:
     - İletilerde **kötü amaçlı olabilecek bilinmeyen URL'ler için eylemi seçin öğesini açma.**
     - Kuruluş **içinde gönderilen iletilere güvenli bağlantılar uygula öğesini seçin.**

  Daha fazla bilgi için bkz [Kasa. Office 365 için Microsoft Defender'da Bağlantılar Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
