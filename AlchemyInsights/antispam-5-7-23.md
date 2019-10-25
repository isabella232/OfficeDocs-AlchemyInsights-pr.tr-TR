---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682336"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Hata kodu 5.7.23 için e-posta teslim sorunlarını düzeltme

Web'de herkese açık bir SPF veya DNS kayıt denetleyicisi olarak etki alanınız için SPF DNS kaydını doğrulayın.

Giden iletinin Office 365 tarafından spam olarak tanımlanmadığını ve [Yüksek Riskli Teslim Havuzu'ndan](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)yönlendirildiğini doğrulayın. Yüksek Riskli Teslim Havuzundaki iletiler SPF denetimlerini geçmez ve bu nedenle hedef e-posta kuruluşu tarafından kabul edilmez.

Sorun devam ederse, e-posta göndermeye çalıştığınız posta ana bilgisayar yöneticisiyle iletişime geçmeniz gerekebilir. Geri dönen iletide bulunan ayrıntılı dış hataya dikkat edin.  Office 365 desteği daha fazla yardımcı olamayabilir.