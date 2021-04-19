---
title: SMTP kimlik doğrulama sorunlarını çözme
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826435"
---
# <a name="solving-smtp-authentication-issues"></a>SMTP kimlik doğrulama sorunlarını çözme

SMTP e-postası göndermeye çalışırken 5.7.57 veya 5.7.3 hataları alıyor ve bir istemci veya uygulamayla kimlik doğrulama hatası alıyorsanız, denetlemeniz gereken birkaç şey vardır:

- Kimliği doğrulanmış SMTP gönderimi kiracınız veya kullanmaya istediğiniz posta kutusunda devre dışı bırakılmış olabilir (her iki ayarı da kontrol edin). Daha fazla bilgi için bkz. [Kimliği doğrulanmış istemci SMTP gönderimi etkinleştirme veya devre dışı bırakma.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Kiracınız [için Azure Güvenlik Varsayılanları'nın](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) etkinleştirildiğinden emin olun; etkinleştirilirse, temel kimlik doğrulamasını kullanan SMTP kimlik doğrulaması (eski olarak da bilinir; kullanıcı adı ve parola kullanır) başarısız olur.
