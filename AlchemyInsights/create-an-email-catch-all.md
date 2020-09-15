---
title: Tümünü yakala
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713006"
---
# <a name="create-an-email-catch-all"></a>Tümünü yakala

Tümünü yakala 'nın kullanımı kesinlikle önerilmez. Gönderene geri sıçrama sağlamak daha iyidir, gönderenlere ileti teslim edilebilmeleri için iletileri adreslenmiş olarak teslim edilemedi. İzlenen posta kutusunu yalnızca önceden geçerli olan e-posta adresleriyle da sınırlayabilirsiniz. 

Tüm catch posta kutuları istenmeyen bir istenmeyen posta alır ve yakın zamanda izlenmediğini de doldurabilir. (Alan sınırlamaları vardır.) 

Devam etmeye karar verirseniz, şu adımları izleyin:

1. "Tüm alıcı türleri" & dinamik dağıtım grubu oluşturun.

2. E-postaları yakalamak için adanmış bir posta kutusu oluşturun (örneğin, catchall@domain.com.

3. İlgili etki alanı için, DomainType 'ı "ınternalrelay" olarak ayarlayın. Daha sonra tümünü kaldırırsanız, etki alanını yetkili olarak ayarladığınızdan emin olun.

4. Şu şekilde bir mailflow aktarım kuralı oluşturun:

    - Gönderen "kuruluşun dışına" ise
    - İletiyi Catchall@domain.com 'e yönlendirme
    - Alıcının üyesi olması dışında (dağıtım grubu tüm üyeleri içerir)
    - Dinamik dağıtım grubuna yeni posta kutularının eklendiğini doğrulama
