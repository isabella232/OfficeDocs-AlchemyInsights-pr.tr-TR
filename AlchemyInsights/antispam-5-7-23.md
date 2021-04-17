---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821431"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme

Web'de genel kullanıma açık bir SPF veya DNS kayıt denetleyicisinde etki alanınız için SPF DNS kaydını doğrulayın.

Giden iletinin Microsoft tarafından istenmeyen posta olarak tanım olmadığını ve Yüksek Riskli Teslim Havuzu aracılığıyla [yönlendirildi doğrulayın.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Yüksek Riskli Teslim Havuzu'daki iletiler SPF denetimlerinden geçirilecek ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmayacak.

Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayarının yöneticisine başvurabilirsiniz. Geri dönen iletide kullanılabilen ayrıntılı dış hatayı not alabilirsiniz. Microsoft desteği daha fazla yardımcı olabilir.
