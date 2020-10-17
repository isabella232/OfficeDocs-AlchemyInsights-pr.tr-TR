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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478331"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-posta iletmeyi engelleme veya engellemeyi kaldırma

Belirli bir posta kutusu için e- [posta iletmeyi etkinleştirmek](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)veya devre dışı bırakmak için

Kiracı düzeyinde, dış iletme denetimi giden istenmeyen posta ilkesi kullanılarak yapılır. Güvenlik ve Uyumluluk Merkezi 'nden giden istenmeyen posta Filtresi politikasını [buradan](https://protection.office.com/antispam) veya [Get-HostedOutboundSpamFilterPolicy komutunu](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)kullanarak denetleyebilirsiniz.

Aşağıdaki hatayı alıyorsanız: **"550 5.7.520 erişim reddedildi, kuruluşunuz dış iletmeye izin vermiyor"**, lütfen Ilkenin dış Otomatik iletmeyi etkinleştirecek şekilde yapılandırıldığından emin olun.

**Not:** Varsayılan giden istenmeyen posta Filtresi ilkeleriniz için dış otomatik Iletme devre dışı tutulmasını ve yalnızca bu kullanıcılar için özel bir ilke oluşturarak yalnızca dış yönlendirmeyi gerektiren kullanıcıları etkinleştirmesini öneririz. [Office 365 ' de dış e-posta Iletmeyi yapılandırmada](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)daha fazlasını okuyabilirsiniz.