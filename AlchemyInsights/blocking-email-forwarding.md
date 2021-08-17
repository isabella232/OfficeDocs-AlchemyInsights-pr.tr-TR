---
title: 726 E-posta iletmeyi engelleme
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059652"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>E-posta iletmeyi engelleme veya engelini kaldırma

Belirli bir posta kutusunda e-posta iletmeyi etkinleştirmek veya devre dışı bırakmak için bkz. [E-posta iletmeyi yapılandırma.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Kiracı düzeyinde, dış iletme denetimi giden istenmeyen posta ilkesi kullanılarak yapılır. Giden istenmeyen posta filtresi ilkesine buradan veya [](https://protection.office.com/antispam) [Get-HostedOutboundSpamFilterPolicy komutunu kullanarak bakabilirsiniz.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Aşağıdaki hatayı alıyorsanız: **"550 5.7.520 Erişim reddedildi,** Organizasyonunız dış iletmeye izin vermiyor" , lütfen ilkenin Dış Otomatik iletmeyi etkinleştirmek üzere yapılandırıldığından emin olun.

**Not:** Dış Otomatik Iletme özelliğini varsayılan giden istenmeyen posta filtresi ilkeniz üzerinde devre dışı tutmanız ve yalnızca dış iletme ihtiyacı olan kullanıcılar için özel bir ilke oluşturarak bu ilkeyi etkinleştirmeniz önerilir. Dış e-posta [iletmeyi yapılandırma makalesinde daha fazla bilgi Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)