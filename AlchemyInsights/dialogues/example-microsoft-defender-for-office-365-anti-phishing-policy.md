---
title: Office 365 için Microsoft Defender kimlik avı önleme ilkesi örneği
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695638"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Office 365 için Microsoft Defender kimlik avı önleme ilkesi örneği

Bu ayarlar, Etki Alanı ve CEO olarak *adlandırılan ilkeyi etkinleştirir.* Bu ilke, hem kullanıcı hem de etki alanı korumasını kimliğe bürünme karşı sağlar ve ardından bu ilkeyi etki alanı içindeki kullanıcılar tarafından alınan tüm e-postalara uygular. İlk olarak, ilkeyi oluşturmak için aşağıdaki bilgileri ekleyin:

- **Ad**: Etki alanı ve CEO **Açıklaması**: CEO'nun ve etki alanınız kimliğine bürünülmemelerini sağlar.
  **Uygulandığı yer:** Alıcı **etki alanını seçin.** Bunların **herhangi biri altında,** **Seç'i** seçin ve sonra da bir etki alanı seçin. + **Ekle'yi seçin.** Listede etki alanının adının yanındaki onay kutusunu seçin *(örneğin,* contoso.com) ve ardından Ekle'yi **seçin.** **Bitti'yi seçin.**
- İlke oluşturulduktan sonra, aşağıdaki seçenekleri kullanarak ilkede ince ayarlamalar yapabilirsiniz:
  - **Korumak için kullanıcı ekleme:** Bu örnekte, CEO'nun e-posta adresini en azından ekleyin.
  - **Korumak için etki alanları ekleyin:** CEO'nun ofisini içeren kuruluş etki alanını ekleyin.
  - **Eylemleri seçin:** **E-posta** kimliğine bürünülen bir kullanıcı tarafından gönderilirse, iletiyi başka bir e-posta adresine yönlendir'i seçin ve güvenlik yöneticisinin e-posta adresini girin (örneğin, *securityadmin@contoso.com).* **E-posta kimliğine bürünülen bir etki alanı tarafından gönderilirse,** **iletiyi karantinaya alın'ı seçin.**
  - **Posta kutusu** zekası: Yeni bir kimlik avı önleme ilkesi oluşturmak için varsayılan olarak bu seçenek seçilidir. En iyi sonuçları elde **etmek için bu** ayarı Açık bırakın.
  - **Güvenilen gönderenleri ve etki alanlarını ekleyin:** Bu örnekte, geçersiz kılmaları tanımlamayın.
- Ayarlarınızı gözden geçirerek uygun şekilde Bu ilkeyi **oluştur veya** **Kaydet'i** seçin.

Daha fazla bilgi edinmek için [Microsoft 365'te kimlik avı önleme ilkelerine bakın.](https://go.microsoft.com/fwlink/?linkid=2092235)
