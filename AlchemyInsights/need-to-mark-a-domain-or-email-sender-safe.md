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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025630"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Etki alanını veya e-posta göndereni güvenli olarak işaretlemeniz mi gerekiyor?

- Güvenli gönderen **listelerinin kullanılması önerilmez,** çünkü kuruluş istenmeyen posta, kimlik avı ve kimlik avı saldırılarına karşı açılır.
- Bununla birlikte, bir iş gereksinimi varsa, **bunun için Posta** Posta Flow **[kuralları'nın kullanılması](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** önerilir. Kılavuzlarımız gönderen kimlik doğrulamasını (etki alanı göndermenin kimlik doğrulamasının kimlik doğrulaması olmadığını doğrular) sağlar. **Not:** İstenmeyen posta filtreleme özel durumları güvenlik saldırılarına karşı kurumlarınızı aç etkileyecer, bunun için güvenilir gönderen listeleri kullanarak hatalı pozitif sonuç yönetimine izin veririz. Kullanıcınız yanlışlıkla istenmeyen veya gereksiz e-posta olarak işaretlenmiş iletileri alırsa, lütfen İletileri ve **[dosyaları Microsoft'a rapor edin.](https://protection.office.com/reportsubmission)**
- Kasa Gönderenler tüm istenmeyen postayı, kimlik avını ve kimlik  avını (SPF, DKIM, DMARC) atlayamalarından dolayı Outlook, İzin verilen gönderenler listesi veya istenmeyen posta önleme ilkelerinden izin verilen etki alanı listesinde yer alan gönderenler engel olmalıdır. Bu yöntem, yalnızca geçici test için en iyi yöntemdir.
- Belirli bir e-postanın Antispam değerlendirmesini atlayan bir e-postanın doğrulanması, "X-Forefront-Antispam-Report" ileti üst bilgisi (SFV:SFE, SFV:SKA, SFV:SKN) denetlenerek yapılabilir, bkz. İstenmeyen posta iletisi **[üstbilgileri.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Microsoft müşterilerimizin varsayılan olarak güvenli güvenliğini [sağlamak](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)istediği için, bazı kiracı geçersiz kılmaları kötü amaçlı yazılım ve yüksek güvenli kimlik avı için uygulanmaz. Bu geçersiz kılmalar şunlardır: o İzin verilen gönderenler listeleri veya izin verilen etki alanı listeleri (istenmeyen posta önleme ilkeleri) Outlook Kasa Gönderenler o IP İzin Listesi (bağlantı filtreleme) 
- Kimlik avı iletisinin filtreyi atlayarak yüksek güvene sahip kimlik avı iletisine izin veren tek geçersiz Exchange akışı kurallarıdır (aktarım kuralları olarak da bilinir). Filtreyi atlamak üzere posta akış kurallarını kullanmak için bkz. İletilerde istenmeyen posta güven düzeyi **[(SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** ayarlamak için posta akış kurallarını kullanma .