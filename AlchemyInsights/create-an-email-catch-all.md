---
title: Tümeği yakalama e-posta sıyrık oluşturma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286311"
---
# <a name="create-an-email-catch-all"></a>Tümeği yakalama e-posta sıyrık oluşturma

Bir yakalama tüm kullanımı şiddetle önerilmez. Gönderene, gönderenlere, iletilerinin adreslendirilen şekilde teslim edilemediğini bildirilmesi ne kadar önemli yse, bu nedenle işlem yapabilmeleri için geri sıçrama sağlamak daha iyidir. Ayrıca, izlenen posta kutusunu yalnızca daha önce geçerli olan e-posta adreslerini yakalamak için sınırlayabilirsiniz. 

Herhangi bir yakalamak tüm posta kutusu spam iyi bir anlaşma alırsınız ve sonunda yakından izlenmezeğer doldurabilir. (Alma sınırları vardır.) 

Devam etmeye karar verirseniz, aşağıdaki adımları izleyin:

1. Dinamik Dağıtım Grubu oluşturma & "Tüm Alıcı Türleri" içerir.

2. Örneğin, catchall@domain.com e-postaları yakalamak için özel bir Posta Kutusu oluşturun.

3. Belirli etki alanı için DomainType'ı "InternalRelay" olarak ayarlayın. Daha sonra tüm yakalamayı kaldırırsanız, etki alanını Yetkili'ye geri ayarladığınızdan emin olun.

4. Posta Akışı Aktarım Kuralı'nı aşağıdaki gibi oluşturun:

    - Gönderen "Kuruluş Dışında" ise
    - İletiyi Catchall@domain.com'a yönlendirme
    - Alıcı allusers@domain.com üyesi yse (Dağıtım Grubu tüm üyeleri içerir)
    - Dinamik Dağıtım Grubuna yeni posta kutularının eklenmesini doğrulamayı sağlamak
