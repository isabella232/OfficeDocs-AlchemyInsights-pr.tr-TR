---
title: Kimlik avı önleme Office 365 için Microsoft Defender örneği
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035026"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Kimlik avı önleme Office 365 için Microsoft Defender örneği

Bu ayarlar Domain and CEO adlı *bir ilkeyi etkinleştirir.* Bu ilke, hem kullanıcı hem de etki alanı kimliğine karşı koruma sağlar ve ardından ilkeyi etki alanı içindeki kullanıcılar tarafından alınan tüm e-postalara uygular. İlk olarak, ilkeyi oluşturmak için aşağıdaki bilgileri ekleyin:

- **Ad:** Etki alanı ve CEO **Açıklaması**: CEO'nun ve etki alanınız kimliğine bürünülmemelerini sağlar.
  **Şu şekilde uygulanır:** Alıcı **etki alanı öğesini seçin.** Bu **seçeneklerden herhangi biri altında,** **Seç öğesini** seçin ve sonra da bir etki alanı seçin. **+ Ekle öğesini seçin.** Listede etki alanı adının yanındaki onay kutusunu seçin *(örneğin,* contoso.com ) ve ekle'yi **seçin.** Bitti **öğesini seçin.**
- İlke oluşturulduktan sonra, aşağıdaki seçenekleri kullanarak ilkede ince ayarlamalar yapabilirsiniz:
  - **Korumak için kullanıcı ekleme:** Bu örnekte, CEO'nun e-posta adresini en azından ekleyin.
  - **Korumak için etki alanları ekleyin:** CEO'nun ofisini içeren kuruluş etki alanını ekleyin.
  - **Eylemleri seçin:** **E-posta** kimliğine bürünülen bir kullanıcı tarafından gönderilirse için, İletiyi başka bir e-posta adresine yeniden yönlendir'i seçin ve güvenlik yöneticisinin e-posta adresini girin *(örneğin, securityadmin@contoso.com).* **E-posta kimliğine bürünülen bir etki alanı tarafından gönderilirse için İletiyi** **karantinaya alın öğesini seçin.**
  - **Posta kutusu** zekası: Varsayılan olarak, yeni bir kimlik avı önleme ilkesi 7 oluşturmak için bu seçenek seçilidir. En iyi sonuçları elde **etmek için bu** ayarı Açık bırakın.
  - **Güvenilen gönderenleri ve etki alanlarını ekleme:** Bu örnekte, geçersiz kılmalar tanımlamayın.
- Ayarlarınızı gözden geçirmenizin ardından, Uygun şekilde Bu ilkeyi **oluştur'a veya** **Kaydet'e** tıklayın.

Daha fazla bilgi için [bkz. Kimlik avıyla mücadele ilkeleri Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
