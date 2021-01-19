---
title: Uygulamalarda oturum açma sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901322"
---
# <a name="issues-signing-in-to-applications"></a>Uygulamalarda oturum açma sorunları

Kullanıcı oturum açma ile ilgili sorunları saptamak veya tanılamak için aşağıdaki adımları uygulayın:

1. [Oturum açma tanılaması](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)'nı başlatın.
2. Kullanıcı, uygulama, oturum açma zamanı, istek kimliği veya bağıntı kimliği hakkında sahip olduğunuz Ayrıntıları girerek çözümlenecek olayı bulun.
3. Herhangi bir değişiklik yapılması gerekirse, ne olduğunu ve değişiklik yapmak için uygulayabileceğiniz eylemleri gösteren Tanılama sonuçlarını gözden geçirin.

Uygulamalarda oturum açarken karşılaşabileceğiniz bazı yaygın sorunlar şunlardır:

1. Siz veya Kullanıcı **bir Azure AD oturum açma işlemini tamammıştır, ancak beklenmeyen bir istem görür;** bir uygulamada oturum açarken ve bir [uygulamaya izin](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)uygularken beklenmeyen [onay istemi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
2. Siz veya bir Kullanıcı **doğrudan bir uygulamada oturum açtı, ancak özel portalında veya Access panelindeki bir derin bağlantısından oturum açamıyor**. [Azure AD uygulamalarımdan gelen bir uygulamada oturum açma sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)konusuna bakın.
3. Siz veya bir Kullanıcı **Azure AD oturum açma işlemini tamamladı, ancak uygulama bir hata iletisi görüntülüyor ve kullanıcının oturum açma akışını bitirmesine izin vermez**: sorun, UYGULAMANıN Azure AD 'nin verdiği yanıtı kabul etmediği oldu. Sorunu gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) izleyin.
4. Siz veya Kullanıcı **parola çoklu oturum açma için yapılandırılmış Galeri dışı bir uygulamada oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) izleyin.
5. Siz veya Kullanıcı **parola çoklu oturum açma için yapılandırılmış bir Azure AD Galerisi uygulamasında oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) izleyin.
6. Siz veya bir Kullanıcı **Microsoft uygulamasında oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) izleyin.
7. Siz veya Kullanıcı **federe çoklu oturum açma için yapılandırılmış Galeri olmayan bir uygulamada oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) izleyin.
8. Siz veya Kullanıcı **federe çoklu oturum açma için yapılandırılmış bir Azure AD Galerisi uygulamasında oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) izleyin.
9. Siz veya bir Kullanıcı **özel geliştirildiği bir uygulamada oturum açamıyor**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) izleyin.
10. Siz veya Kullanıcı **Azure AD uygulaması proxy 'sini kullanarak şirket içi bir uygulamada oturum açamaz**: sorun gidermek için [Bu adımları](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) izleyin.

