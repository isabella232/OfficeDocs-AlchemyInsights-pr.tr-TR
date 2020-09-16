---
title: Web üzerinde Outlook 'ta S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772318"
---
# <a name="encrypt-email-messages-in-outlook"></a>Outlook 'ta e-posta iletilerini şifreleme

Microsoft 365 Ileti şifreleme, Azure Information Protection 'ın bir parçası olan Microsoft Azure Rights Management (Azure RMS) üzerine kurulmuştur. Aboneliğiniz Azure Rights Management veya Azure Information Protection içeriyorsa, hak yönetimi hizmetini **etkinleştirmek veya etkinleştirmek için herhangi bir işlem yapmanız gerekmez** .

Müşteri geri bildirimlerine bağlı olarak, varsayılan olarak kiracınızda belirli tür duyarlı bilgileri içeren giden e-postayı otomatik olarak şifreleyemiyoruz. Bunun yerine yourselves bunu nasıl yapabileceğiniz hakkında ayrıntılı yönergeler sunuyoruz. Hassas bilgilerin şifrelenmesinde bir taşıma kuralı oluşturma hakkında ek bilgi için [Bu makaleye](https://aka.ms/OmeEtr)bakın.

- Web üzerinde Outlook (eski adı **OWA**) kullanılıyorsa: e-posta iletisi oluştururken, yalnızca OWA 'da **korumayı** tıklatın. "İletme" izni uygulanır. **Izni Değiştir** 'i tıklatın ve yalnızca iletiyi şifrelemek için **şifrele** 'yi seçin.

- **Outlook istemcisi**kullanılıyorsa: Outlook 2013 veya 2016 veya Mac için Outlook 2016 ' den şifrelenmiş bir ileti göndermek için **Seçenekler**  >  **izinler**'i seçin ve sonra da ihtiyacınız olan koruma seçeneğini belirleyin.

- Belirli alıcılara veya dış iş ortağı kuruluşlara gönderilen **tüm e-postaları otomatik olarak şifrelemek** Için, Exchange Yönetim merkezinde bir posta akışı aktarım kuralı oluşturmanız gerekir. Ayrıntılı yönergeler [Bu destek makalesinde](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)sağlanmaktadır.

