---
title: Etki alanı veya e-posta gönderenini güvenli olarak işaretlemelisiniz mi gerekiyor?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803265"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Etki alanı veya e-posta gönderenini güvenli olarak işaretlemelisiniz mi gerekiyor?

- Kuruluşunuzu istenmeyen posta, sızdırma ve sızdırma saldırılarına karşı açtığından **güvenli gönderen listelerinin kullanımı önerilmez** .
- Bununla birlikte, iş gereksinimi varsa, bunun için **[posta akış kurallarını](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** kullanmanızı **öneririz** . Kılavuzumuz, Gönderen kimlik doğrulamasını garantiler (etki alanı göndermeyi doğrular.). **Not**: istenmeyen filtreleme özel durumları kuruluşunuzun güvenlik saldırılarına karşı açabildiğinden, güvenli gönderen listelerini kullanarak yanlış pozitif durumları yönetmeniz önerilmez. Kullanıcılarınız iletileri yanlışlıkla istenmeyen posta veya gereksiz e-posta olarak alıyorsa, lütfen **[iletileri ve dosyaları Microsoft 'A bildirin](https://protection.office.com/reportsubmission)**.
- Gönderenler, istenmeyen posta önleme, sızma ve bir istenmeyen postayı devre dışı bırakabilir ve Gönderen kimlik **should be avoided** doğrulaması (SPF, CıKIM, DMARC) gibi Bu yöntem yalnızca geçici test için kullanılır.
