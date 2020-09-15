---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717345"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme

Web üzerinde genel kullanıma sunulan bir SPF veya DNS kayıt denetleyicisinde etki alanınızın SPF DNS kaydını doğrulayın.

Giden iletinin Microsoft tarafından istenmeyen posta olarak tanımlandığını ve [yüksek riskli teslim havuzu](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)aracılığıyla yönlendirildiğini doğrulayın. Yüksek riskli teslim havuzundaki mesajlar SPF denetimlerini geçirmez ve bu nedenle hedef e-posta organizasyonu tarafından kabul edilmez.

Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayarının yöneticisine başvurmanız gerekebilir. Sıçrama iletisindeki ayrıntılı dış hata hatasını not alın. Microsoft desteği daha fazla yardımcı olabilir.
