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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118003"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>E-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama

Seçenekleriniz ve adımlar hakkında bilgi edinmek için bkz. [Microsoft 365 kullanarak e-posta göndermek için bir çok işlevli cihazı veya uygulamayı ayarlama](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Yakın zamanda çalışmayı durduran bir cihazınız veya uygulamanız varsa en yaygın sorunlar:

- **SMTP Auth istemci gönderimi kullanılırken kimlik doğrulama ile ilgili hatalar** Yakın zamanda SMTP Kimlik Doğrulaması'nın çalışma yöntemiyle ilgili bazı değişiklikler yaptık. Sorunları çözme hakkında daha fazla bilgi için, Microsoft 365 veya LOB kullanarak e-posta gönderen [yazıcılar,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)tarayıcılar ve LOB uygulamalarıyla ilgili sorunları düzeltme bölümünün kimlik doğrulama başarısız Office 365.
- **Güvenli bir veri bağlantısı yaparken yalnızca TLS 1.2 sürümünü kabul Office 365** Güvenli bağlantı (TLS) kullanıyorsanız, uygulama cihazınızın TLS 1.2'yi desteklediğine emin olun. Daha fazla bilgi için bkz. [TlS 1.2 için Office 365 ve Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Diğer sorunlar ve çözümler için bkz. Microsoft 365 veya LOB kullanarak e-posta gönderen [yazıcılar, tarayıcılar ve LOB Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Etkilenen cihazları görmek için [SMTP Kimlik Doğrulama İstemcileri raporuna](https://protection.office.com/mailflow/dashboard) gidin.

**Not:** Exchange Online toplu posta senaryolarına uyum sağlar. Toplu ticari e-posta göndermek için (örneğin, müşteri bültenleri), bu hizmetlerde özelleştirilmiş üçüncü taraf sağlayıcıları kullansanız gerekir.
