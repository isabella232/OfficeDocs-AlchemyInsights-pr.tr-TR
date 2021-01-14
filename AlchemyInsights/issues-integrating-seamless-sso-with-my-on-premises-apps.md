---
title: Şirket içi uygulamalarınızla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunlar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868770"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Şirket içi uygulamalarınızla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunlar

Şirket içi uygulamalarla kesintisiz SSO 'yu tümleştirmeyle ilgili sorunları gidermek için aşağıdakileri yapın:

**Önerilen adımlar**

1. **Uygulama ara sunucusu aracılığıyla çoklu oturum açma** için bir **Şirket içi uygulama** yapılandırmak üzere, [uygulama proxy 'si Ile çoklu oturum açma için parola](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)oluşturma konusuna bakın.
1. **Uygulama proxy 'si sorunlarını giderme**: uygulama proxy bağlayıcıları 'nın doğru yapılandırılıp yapılandırılmadığını belirlemek Için, [uygulama ara](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) Uygulamaya bağlanma konusunda hala sorun yaşıyorsanız, [uygulama proxy 'si uygulama sorunlarını ayıklamada](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)sorun giderme adımlarını izleyin. [CORS sorunlarını](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) aşağıdaki tarayıcı hata ayıklama araçlarını kullanarak tanımlayabilirsiniz:
    1. Tarayıcıyı başlatın ve Web uygulamasına gidin.
    1. Debug konsolunu görüntülemek için **F12** tuşuna basın.
    1. İşlemi yeniden oluşturmaya çalışın ve konsol iletisini gözden geçirin. CORS ihlaliyle ilgili bir konsol hatası veriyor.
    1. Uygulamanızın kimlik doğrulaması için login.microsoftonline.com 'a yönlendirdiği ve erişim belirtecinin süresi dolduğunda bazı CORS sorunları çözülebilir. CORS çağrısı başarısız olur. Bu senaryo için geçici bir çözüm olan erişim belirtecinin kullanım süresini uzatmak, kullanıcının oturumu sırasında süresinin dolmasını önleyecek şekilde. Bunu yapma hakkında daha fazla bilgi için [Microsoft Identity platformunda yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)konusuna bakın.

**Önerilen belgeler**

- [Uygulama proxy uygulamasında çoklu oturum açmayı yapılandırma](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Uygulama proxy 'Si ile şirket içi uygulamalar için SAML tekli oturum açma](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory uygulama proxy CORS sorunlarını anlama ve çözme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Uygulama proxy 'Si için Kerberos kısıtlı temsilci yapılandırmalarında sorun giderme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)