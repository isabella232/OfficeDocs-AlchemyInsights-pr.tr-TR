---
title: Etki alanını veya e-posta göndereni güvenli olarak işaretlemeniz mi gerekiyor?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792152"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Etki alanını veya e-posta göndereni güvenli olarak işaretlemeniz mi gerekiyor?

- Güvenli gönderen **listelerinin kullanılması önerilmez,** çünkü kuruluş istenmeyen posta, kimlik avı ve kimlik avı saldırılarına karşı açılır.
- Bununla birlikte, bir iş gereksinimi varsa, **bunun için Posta** **[Akış Kuralları'nın kullanılması](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** önerilir. Kılavuzlarımız gönderen kimlik doğrulamasını (etki alanı göndermenin kimlik doğrulamasının kimlik doğrulaması olmadığını doğrular) sağlar. **Not:** İstenmeyen posta filtreleme özel durumları güvenlik saldırılarına karşı kurumlarınızı aç etkileyecer, bunun için güvenilir gönderen listeleri kullanarak hatalı pozitif sonuç yönetimine izin veririz. Kullanıcınız yanlışlıkla istenmeyen veya gereksiz e-posta olarak işaretlenmiş iletileri alırsa, lütfen İletileri ve **[dosyaları Microsoft'a rapor edin.](https://protection.office.com/reportsubmission)**
- Outlook'ta Güvenilir Gönderenler, İzin verilen gönderenler listesi  veya istenmeyen posta önleme ilkelerde izin verilen etki alanı listesi, gönderenler tüm istenmeyen postayı, kimlik avını ve kimlik avını (SPF, DKIM, DMARC) atlayamalarından kaçınılmalıdır. Bu yöntem, yalnızca geçici test için en iyi yöntemdir.
