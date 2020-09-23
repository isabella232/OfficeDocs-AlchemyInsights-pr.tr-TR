---
title: 726 e-posta iletmeyi engelliyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219875"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-posta iletmeyi engelleme veya engellemeyi kaldırma

Belirli bir posta kutusu için e- [posta iletmeyi etkinleştirmek](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)veya devre dışı bırakmak için

Kiracı düzeyinde, dış iletme denetimi giden istenmeyen posta önleme ilkesi kullanılarak yapılır. Kapalı veya otomatik olarak ayarlanmışsa, "550 5.7.520 erişimi reddedildi, kuruluşunuz dış iletmeye izin vermiyor" hatası ile e-posta iletmeyi engelleyebilir. Ardından, yönlendirme engellenmiş olarak ayarlanmışsa, bu hata, kullanıcılarınızın göreceği hatadır.

İletme engellendiyse, lütfen ilkenin dış otomatik Iletimi etkinleştirecek şekilde yapılandırıldığından emin olun. Giden Istenmeyen posta Filtresi Ilkesini güvenlik ve Uyumluluk Merkezi 'nden denetleyebilir veya Command-HostedOutboundSpamFilterPolicy | fl Name, AutoForwardingMode. Otomatik Iletme engellemesi 'ni ayarlamak istiyorsanız, ilkenin durumunu şimdi size bildirir.

Not: Varsayılan giden Istenmeyen posta Filtresi ilkeleriniz için dış otomatik Iletme devre dışı tutulmasını ve yalnızca bu kullanıcılar için özel bir ilke oluşturarak yalnızca dış yönlendirmeyi gerektiren kullanıcıları etkinleştirmesini öneririz. [Office 365 ' de dış e-posta Iletmeyi yapılandırmada](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)daha fazlasını okuyabilirsiniz.