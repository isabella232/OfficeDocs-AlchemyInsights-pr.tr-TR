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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405684"
---
# <a name="authentication-app"></a>Kimlik doğrulama uygulaması

Genel Yöneticiyseniz Oturum Açma Tanılama'yı kullanarak kullanıcı oturum açmayla ilgili ne olduğunu hemen bulabilir veya sorunları [tanıabilirsiniz.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Tanılamayı başlatmak için "Tanılamayı[Başlat"](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)düğmesine tıklayın. 
1. Kullanıcı, uygulama, oturum açma zamanı, kimlik isteği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntıları girerek analiz etmek için olayı bulun.
1. Ne olduğunu ve gerekirse değişiklik yapmak için hangi eylemleri gerçekleştirebilirsiniz ayrıntılarını gösteren tanılama sonuçlarını gözden geçirebilirsiniz.

**Uygun olan senaryoyu kontrol edin:**

1. Kullanıcı Microsoft Authenticator uygulamasında bir anında bildirim alsa bile, Engelleme ve kullanıcıların engellemesini kaldırma konusunda açıklandığı gibi MFA engellenen kullanıcıların altında [gösterilmeyebileceklerini doğrulayın.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Kullanıcı MFA için engellenmiş ancak bir anında bildirim almayacaksa, Microsoft Authenticator uygulamasını açabilir ve bu da bekleyen onay isteklerini çeker.
1. Alternatif bir oturum açma yöntemi olarak, kullanıcı başka bir yolla Oturum aç'a tıklar ve mobil uygulamamdan bir doğrulama kodu kullanmayı seçebilir.
1. Microsoft Authenticator Uygulaması, birçok kullanıcı için kullanılabilen tek yöntemdir. [Güvenlik varsayılanları hakkında daha fazla bilgi edinin,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator Uygulaması hakkında sık](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) sorulan sorular ve bunları çözme hakkında SSS bölümünü inceleyin.
 
**Önerilen Videolar**

[Authenticator Uygulamasını yeni bir telefonda (2 dakika) ayarlama.](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
