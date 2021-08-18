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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897488"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Otomatik e-posta iletmeyi engelleme veya engelini kaldırma

Belirli bir posta kutusunda e-posta iletmeyi etkinleştirmek veya devre dışı bırakmak için bkz. [E-posta iletmeyi yapılandırma.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Yöneticiler, giden istenmeyen posta ilkelerini kullanarak kuruluş için [dış iletmeyi kontrol ediyor olabilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Microsoft 365 Defender portalında giden istenmeyen posta ilkelerini, <https://security.microsoft.com/antispam> Exchange Online PowerShell'de [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) cmdlet'ini kullanarak yönetirsiniz.

Aşağıdaki hatayı alırsanız: **"550 5.7.520 Erişim reddedildi,** Organizasyonunız dış iletmeye izin vermiyor" iletisini alırsanız, ilkenin dış otomatik iletili iletileri etkinleştirmek üzere yapılandırıldığından emin olun.

**Not:** Varsayılan giden istenmeyen posta filtresi ilkeniz (otomatik dış iletme engellendi; iç otomatik iletme hala çalışıyor) için otomatik iletme kuralları ayarı için denetlenen varsayılan Otomatik **-** Sistem değerini öneririz.  Özel giden istenmeyen posta filtresi ilkeleri oluşturmalı ve Açık - Yönlendirme yalnızca dış otomatik **e-posta** iletmesi gereken kullanıcılar için etkinleştirilmiştir. Daha fazla bilgi için [bkz. Dış e-posta iletmeyi Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
