---
title: Koşullu erişim sorunları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069984"
---
# <a name="conditional-access-issues"></a>Koşullu erişim sorunları

**Oturum Açma Tanılama ile ilgili sorunları çözme**

Oturum Açma Tanılama'yı kullanarak, oturum açmayla ilgili ne olduğunu veya kullanıcı oturum açmayla ilgili [sorunları tanılamayı hızlı bir şekilde bulabilirsiniz:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Oturum Açma Tanılama'yı başlatma.
1. Kullanıcı, uygulama, oturum açma zamanı, istek kimliği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntılara girerek analiz etmek için olayı bulun.
1. Ne olduğunu ayrıntıları ve değişiklik yapmak için hangi eylemleri gerçekleştirebilirsiniz (gerekirse) gösteren tanılama sonuçlarını gözden geçirebilirsiniz.

**Oturum Açma Sorunlarını Giderme Adımları** 

1. Azure AD Oturum Açma sayfasına gidin.
1. Oturum açma bilgilerini kullanıcıya, zaman aralığına, uygulamaya, duruma, istemci uygulamasına, buna göre filtrele.
1. Hangi ilkelerin değerlendirildi görmek için bir oturum açma olayı seçin ve Koşullu Erişim sekmesini görüntüleyin.
1. İlkenin ayrıntılarını görüntülemek ve neden uygulandığını anlamak için ilke satırına tıklayın.

**Koşullu Erişim ilkesi sorunlarını giderme araçları**

- Yalnızca rapor modu kullanıcıları etkilemeden bir ilkeyi değerlendirmenizi sağlar.
- Benzetim aracı, oturum açma olaylarını benzetimini görmenizi ve hangi ilkelerin geçerli olduğunu görmenizi sağlar.
- Analizler raporlama çalışma kitabı her ilkenin gerçek zamanlı etkisini görüntüler.

**Temel Koruma İlkeleri**

Temel Koruma ilkeleri kullanım dışıdır. Bu abonelikler artık zorunlu kılınmayacak ve yakında Azure portaldan kaldırılacaktır. Güvenlik varsayılanlarını [etkinleştirmenizi öneririz.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Koşullu Erişim hakkında daha fazla bilgi için bkz:

[E-postada koşullu erişim için en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu Erişim koşulları](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu Erişim'de Denetimler](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Koşullu Erişim'de Konumlar](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
