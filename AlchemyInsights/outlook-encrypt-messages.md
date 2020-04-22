---
title: Web'de Outlook'ta S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764892"
---
# <a name="encrypt-email-messages-in-outlook"></a>Outlook'ta e-posta iletilerini şifreleme

Microsoft 365 İleti Şifrelemesi, Azure Bilgi Koruması'nın bir parçası olan Microsoft Azure Hakları Yönetimi 'nde (Azure RMS) yerleşiktir. Aboneliğiniz Azure Hakları Yönetimi veya Azure Bilgi Koruması içeriyorsa, Hak Yönetimi Hizmetini **el ile etkinleştirmek veya etkinleştirmek için herhangi bir işlem yapmanız gerekmez.**

Müşteri geri bildirimlerine dayanarak, exchange posta akışı kurallarının varsayılan olarak kiracınızda belirli türde hassas bilgiler içeren giden e-postaları otomatik olarak şifrelemesini etkinleştirmeyeceğiz. Bunun yerine, bunu kendiniz nasıl yapabileceğinize ilişkin ayrıntılı talimatlar salıyoruz. Hassas bilgileri şifrelemek için aktarım kuralının nasıl oluşturulacaaçık ayrıntılar için [bu makaleye](https://aka.ms/OmeEtr)bakın.

- Outlook'u Web'de kullanıyorsanız (eski adıyla **OWA):** Bir e-posta iletisi oluştururken, OWA'da **Koru'yu** tıklatın. Bu " İlerletme" izni geçerli olacaktır. **İzin Değiştir'i** tıklatın ve yalnızca iletiyi şifrelemek için **Şifrele'yi** seçin.

- Outlook **istemcisini**kullanıyorsanız : Outlook 2013 veya 2016'dan veya Mac için Outlook 2016'dan şifreli ileti göndermek için **Seçenekler** > **İzinleri'ni**seçin ve ardından ihtiyacınız olan koruma seçeneğini seçin.

- Belirli alıcılara veya dış iş ortağı kuruluşlarına gönderilen **tüm e-postaları otomatik olarak şifrelemek** için Exchange Yönetici Merkezi'nde bir posta akışı aktarım kuralı oluşturmanız gerekir. Ayrıntılı talimatlar [bu destek makalesinde](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)verilmiştir.

