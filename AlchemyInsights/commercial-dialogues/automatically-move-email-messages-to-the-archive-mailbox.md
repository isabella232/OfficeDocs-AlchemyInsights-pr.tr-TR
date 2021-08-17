---
title: E-posta iletilerini otomatik olarak arşiv posta kutusuna taşıma
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
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059246"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>E-posta iletilerini otomatik olarak arşiv posta kutusuna taşıma

Kullanıcının eski e-postalarını arşiv posta kutusuna otomatik olarak taşımak için ilke şöyle ayarlanır:

1. Kullanıcı için [**bir & posta kutusunun etkinleştirildiğinden**](https://go.microsoft.com/fwlink/p/?linkid=2077143)emin olmak için Güvenlik ve Uyumluluk Verileri  >    >   yönetimi Arşivi'ne gidin. Açmadı ise, **etkinleştir'e ve** **uyarı kutusunda** Evet'e tıklayın.
2. Yönetim merkezi [**Exchange ve bekletme > yönetimi > gidin.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. + simgesini seçin, ardından otomatik olarak **tüm posta kutusuna uygula'ya tıklayın.**
4. Bekletme etiketine bir ad atayın ve Arşive **Taşı'ya seçin.** Bekletme süresi için, istediğiniz saati (örneğin 90 gün) girin. **Kaydet**'e tıklayın.
5. Şimdi bir bekletme ilkesi oluşturun: bekletme **ilkelerini seçin,** yeni bir ilke eklemek için simgeyi seçin.
6. Bekletme ilkesine bir ad atayın, ardından tıklar ve kaydırarak, yeni oluşturduğunuz bekletme etiketini bulup ekleyin. **Kaydet**'e tıklayın.
7. Son olarak, bekletme ilkesi kullanıcın posta kutusuna uygulanır: hala Exchange yönetim merkezinde **alıcılar posta**  >  **kutularına gidin.** İlkeyi uygulamak istediğiniz tüm kullanıcıları seçin,  ardından Düzenle'yi (kalem simgesi) seçin.
8. İletişim kutusunda posta kutusu **özellikleri'ne tıklayın.** Bekletme **ilkesi altında,** yeni oluşturduğunuz ilkeyi Kaydet > **uygulayabilirsiniz.**
9. İlkeyi tüm kullanıcılara uygulama yönergeleri için [bkz. Posta kutularına bekletme ilkesi uygulama.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
