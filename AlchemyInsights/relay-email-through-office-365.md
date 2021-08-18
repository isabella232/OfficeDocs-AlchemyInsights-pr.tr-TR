---
title: Microsoft 365 üzerinden e-posta geçişi
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324382"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>E-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama

Seçenekleriniz ve adımlar hakkında bilgi edinmek için bkz. [Microsoft 365 kullanarak e-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Yakın zamanda çalışmayı durduran bir cihazınız veya uygulamanız varsa en yaygın sorunlar:

- **SMTP Auth istemci gönderimi kullanılırken kimlik doğrulama ile ilgili hatalar** Yakın zamanda SMTP Kimlik Doğrulaması'nın çalışma yöntemiyle ilgili bazı değişiklikler yaptık. Sorunları çözme hakkında daha fazla bilgi için, Microsoft 365 veya Office 365 kullanarak e-posta gönderen [yazıcılar,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)tarayıcılar ve LOB uygulamalarıyla ilgili sorunları düzeltme bölümünün kimlik doğrulama başarısız Office 365.
- **Güvenli bir veri bağlantısı yaparken yalnızca TLS 1.2 sürümünü kabul Office 365** Güvenli bağlantı (TLS) kullanıyorsanız, uygulama cihazınızın TLS 1.2'yi desteklediğine emin olun. Daha fazla bilgi için bkz. Çalışma [Saat ve Saat'de TLS 1.2 Office 365 Office 365 GCC.](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Diğer sorunlar ve çözümler için bkz. [E-posta](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)göndermek için yazıcı, tarayıcı ve LOB uygulamalarıyla ilgili sorunları Microsoft 365 veya Office 365.

Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.

**Not:** Exchange Online toplu posta senaryolarına uyum sağlar. Toplu ticari e-posta göndermek için (örneğin, müşteri bültenleri), bu hizmetlerde özelleştirilmiş üçüncü taraf sağlayıcıları kullansanız gerekir.
