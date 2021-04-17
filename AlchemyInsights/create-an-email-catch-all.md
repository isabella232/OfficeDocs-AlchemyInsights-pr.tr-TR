---
title: Tüm e-posta yakalamaları oluşturma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816220"
---
# <a name="create-an-email-catch-all"></a>Tüm e-posta yakalamaları oluşturma

Tüm avların kullanımı kesinlikle önerilmez. Gönderenlere geri dönmeleri ve iletilerinin adres olarak teslim alınamamasına ve bu şekilde eyleme geçilemelerine izin vermeleri daha iyidir. Ayrıca, izlenen posta kutusunu yalnızca eski geçerli e-posta adreslerini yakalamak için sınırlandırabilirsiniz. 

Tüm posta kutularına gelen tüm yakalamalar çok iyi bir istenmeyen posta alır ve yakın bir şekilde izlenmeyen postaların sayısı zamanla dolabilirsiniz. (Alıcı sınırları vardır.) 

Devam etmeye karar verdiyseniz şu adımları izleyin:

1. "Tüm Alıcı Türleri" & bir Dinamik Dağıtım Grubu grubu oluşturun.

2. E-postaları yakalamak için (örneğin, posta kutunuzu) yakalamak için özel catchall@domain.com.

3. Belirli bir etki alanı için DomainType'ı "InternalRelay" olarak ayarlayın. Tüm yakalamaları daha sonra kaldırırsanız, etki alanını Yetkili olarak ayar mutlaka ayarlayın.

4. Posta Akışı Aktarım Kuralı şöyle oluşturun:

    - Gönderen "Kuruluş Dışında" ise
    - İletiyi Yeniden Yönlendir Catchall@domain.com
    - Alıcının grup üyesi olduğu dışında (allusers@domain.com Grubu tüm üyeleri içerir)
    - Yeni posta kutularının Dinamik Dağıtım Grubuna ek doğrulamak için emin olun
