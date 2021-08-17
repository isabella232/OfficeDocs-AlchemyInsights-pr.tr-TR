---
title: Kimlik doğrulama uygulaması
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082962"
---
# <a name="authentication-app"></a>Kimlik doğrulama uygulaması

Genel Yöneticiyseniz, Oturum Açma Tanılama'yı kullanarak kullanıcı oturum açmayla ilgili ne olduğunu hemen bulabilir veya oturum açma ile ilgili [sorunları tanıabilirsiniz.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. " Tanılamayı Başlat " düğmesine[tıklayarak tanılamayı](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)başlatma. 
1. Kullanıcı, uygulama, oturum açma zamanı, istek kimliği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntılara girerek analiz etmek için olayı bulun.
1. Değişikliklerin ayrıntılarını ve gerekirse değişiklik yapmak için hangi eylemleri gerçekleştirebilirsiniz gibi eylemleri gösteren tanılama sonuçlarını gözden geçirebilirsiniz.

**Uygun olan senaryoyu denetleme:**

1. Kullanıcı Microsoft Authenticator uygulamasında anında bildirim alamasa da, Kullanıcıları engelleme ve engelini kaldırma konusunda açıklandığı gibi MFA engellenen kullanıcıları altında [gösterilmelerini](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)doğrulama .
1. Kullanıcı MFA için engelsizse ancak anında bildirim almayacaksa Microsoft Authenticator uygulamasını açabilir ve bekleyen onay isteklerini çeker.
1. Alternatif oturum açma yöntemi olarak, kullanıcı başka bir yolla oturum aç'a tıklayarak mobil uygulamamdan bir doğrulama kodu kullan'ı da seçebilir.
1. Uygulama Microsoft Authenticator, birçok kullanıcı için kullanılabilen tek yöntemdir. [Güvenlik varsayılanları hakkında daha fazla bilgi edinmek](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)Authenticator [sık](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) sorulan sorular ve bunları nasıl çözeceklerini öğrenmek için Uygulama SSS bölümünü kontrol edin.
 
**Önerilen Videolar**

[Authenticator Uygulamasını yeni bir telefonda (2 dakika) ayarlama.](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
