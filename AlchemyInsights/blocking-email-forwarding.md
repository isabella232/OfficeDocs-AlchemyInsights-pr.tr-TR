---
title: Dış otomatik e-posta iletmeyi engelleme veya engellemesini kaldırma
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315894"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Otomatik e-posta iletmeyi engelleme veya engelini kaldırma

Belirli bir posta kutusunda e-posta iletmeyi etkinleştirmek veya devre dışı bırakmak için bkz. [E-posta iletmeyi yapılandırma.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Yöneticiler, giden istenmeyen posta ilkelerini kullanarak kuruluş için [dış iletmeyi kontrol ediyor olabilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Microsoft 365 Defender portalında giden istenmeyen posta <https://security.microsoft.com/antispam> ilkelerini, Exchange Online PowerShell'de [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) cmdlet'ini kullanarak yönetirsiniz.

Aşağıdaki hatayı alırsanız: **"550 5.7.520 Erişim reddedildi,** Organizasyonunız dış iletmeye izin vermiyor" iletisini alırsanız, ilkenin dış otomatik iletili iletileri etkinleştirmek üzere yapılandırıldığından emin olun.

**Not:** Varsayılan giden istenmeyen posta filtresi ilkeniz (otomatik dış iletme engellendi; iç otomatik iletme hala çalışıyor) için otomatik iletme kuralları ayarı için denetlenen varsayılan Otomatik **-** Sistem değerini öneririz.  Özel giden istenmeyen posta filtresi ilkeleri oluşturmalı ve Açık - Yönlendirme yalnızca dış otomatik **e-posta** iletmesi gereken kullanıcılar için etkinleştirilmiştir. Daha fazla bilgi için [bkz. Dış e-posta iletmeyi Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
