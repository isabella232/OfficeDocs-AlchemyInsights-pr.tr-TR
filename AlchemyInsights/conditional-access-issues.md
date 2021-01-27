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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015005"
---
# <a name="conditional-access-issues"></a>Koşullu erişim sorunları

**Oturum açma tanısı sorunlarını çözme**

[Oturum açma tanılaması](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)kullanarak Kullanıcı oturum açma ile ilgili sorunları hızla bulabilir veya tanılayabilir:

1. Oturum açma tanılaması 'nı başlatın.
1. Kullanıcı, uygulama, oturum açma süresi, istek kimliği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntılara girerek çözümlenecek olayı bulun.
1. Ne olduğunu ve değişiklik yapmak için uygulayabileceğiniz eylemleri (herhangi bir değişiklik gerekiyorsa) gösteren Tanılama sonuçlarını gözden geçirin.

**Oturum açma sorunlarını giderme adımları** 

1. Azure AD oturum açma sayfasına gidin.
1. Oturum açmayı kullanıcıya, zaman aralığına, uygulamaya, duruma, istemci uygulamasına, vb. göre filtreleyin.
1. Hangi ilkelerin değerlendirildiğini görmek için bir oturum açma olayı seçin ve koşullu erişim sekmesini görüntüleyin.
1. İlke ayrıntılarını görüntülemek ve neden uygulandığını anlamak için bir ilkenin satırına tıklayın.

**Koşullu erişim ilkesinde sorun giderme araçları**

- Yalnızca rapor modu kullanıcıları etkilemeden bir ilkeyi değerlendirmenize olanak tanır.
- Durum aracı, oturum açma olaylarının hangi ilkelerin uygulanacağını görmenizi sağlar.
- Öngörüler ve raporlama çalışma kitabı her ilkenin gerçek zamanlı etkisini gösterir.

**Temel koruma Ilkeleri**

Temel koruma ilkeleri kullanımdan kaldırıldı. Artık zorlanmayacak ve Azure portalından yakında kaldırılacaktır. [Güvenlik varsayılanlarını](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirmeyi öneririz.

Koşullu erişimle ilgili daha fazla bilgi için bkz.

[Azure Active Directory 'de koşullu erişim Için en iyi yöntemler](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu erişimde koşullar](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu erişimde denetimler](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Koşullu erişimde konumlar](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
