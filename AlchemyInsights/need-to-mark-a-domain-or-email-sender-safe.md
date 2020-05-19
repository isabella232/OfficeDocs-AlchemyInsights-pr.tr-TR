---
title: Bir etki alanını veya e-posta göndereni güvenli olarak işaretlemeli mi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281239"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Bir etki alanını veya e-posta göndereni güvenli olarak işaretlemeli mi?

- Güvenli gönderen listelerinin kullanılması, kuruluşunuzun spam, kimlik avı ve sahte ciponasyon saldırılarına açık olması **için önerilmez.**
- Ancak, bir iş gereksinimi varsa, bunun için Posta Akışı **Kuralları'nı kullanmanızı öneririz.** **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Kılavuzumuz gönderenin kimlik doğrulamasını sağlar (alan adı göndermenin sahte olmadığını doğrular). **Not**: Spam filtrelemenin istisnaları kuruluşunuzu güvenlik saldırılarına açabileceğinden, güvenli gönderen listeleri kullanarak yanlış pozitif leri yönetmenizi önermiyoruz. Kullanıcınız spam veya önemsiz e-posta olarak yanlış işaretlenmiş iletiler alıyorsa, lütfen **[iletileri ve dosyaları Microsoft'a bildirin.](https://protection.office.com/reportsubmission)**
- Gönderenler tüm spam, sahtekarlık ve kimlik avı korumasını ve gönderen kimlik doğrulamasını (SPF, DKIM, DMARC) atladığı için, Outlook'taki Güvenli Gönderenler, İzin Verilen gönderenler listesinden veya istenmeyen posta önleme politikalarında izin verilen etki alanı listesinden **kaçınılmalıdır.** Bu yöntem en iyi yalnızca geçici sınama için kullanılır.
