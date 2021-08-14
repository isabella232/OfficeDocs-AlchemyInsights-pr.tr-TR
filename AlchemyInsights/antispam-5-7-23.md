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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932189"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme

Web'de genel kullanıma açık bir SPF veya DNS kayıt denetleyicisinde etki alanınız için SPF DNS kaydını doğrulayın.

Giden iletinin Microsoft tarafından istenmeyen posta olarak tanım olmadığını ve Yüksek Riskli Teslim Havuzu aracılığıyla [yönlendirildi doğrulayın.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Yüksek Riskli Teslim Havuzu'daki iletiler SPF denetimlerinden geçirilecek ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmayacak.

Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayarının yöneticisine başvurabilirsiniz. Geri dönen iletide kullanılabilen ayrıntılı dış hatayı not alabilirsiniz. Microsoft desteği daha fazla yardımcı olabilir.
