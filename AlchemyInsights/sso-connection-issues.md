---
title: SSO Bağlantı Sorunları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935206"
---
# <a name="sso-connection-issues"></a>SSO Bağlantı Sorunları

1. Hızlı [Başlangıç'a göz atabilirsiniz: Uygulama kılavuzunun](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) özelliklerini yapılandırarak uygulamanızı yapılandırabilirsiniz.
2. Seçtiğiniz uygulamaya ve Çoklu [oturum açma seçeneğine bağlı](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) olarak, aşağıdaki uygun yönergeleri izleyin:
    - **SAML** **tabanlı** çoklu oturum açma için şirket içi bir uygulamayı yapılandırmak için bkz. Uygulama Ara Sunucusu ile şirket içi uygulamalarda [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)çoklu oturum açma.
    - Bulut uygulamasını **parola tabanlı çoklu** oturum açma için yapılandırmak **için** bkz. Parola çoklu oturum [açma yapılandırma.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Uygulama Ara Sunucusu **aracılığıyla çoklu oturum açma** için şirket içi bir uygulama yapılandırmak için Bkz. Uygulama Ara Sunucusu ile çoklu oturum açma için Parola [kasalama.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
3. **Uygulama Ara Sunucusu** sorunlarını giderme: Uygulama Ara Sunucusu bağlayıcılarının doğru yapılandırıldığından emin olmak için [sorun](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)giderme akışını, Uygulama Ara Sunucu Bağlayıcısı Sorunlarını Ayıkla sorunlarını gözden geçirmeyle başlamanız önerilir. Uygulamaya bağlanma konusunda hala sorun yaşıyorsanız, Uygulama Ara Sunucusu uygulamasındaki hata ayıklama [akışında sorun giderme akışını izleyin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Tarayıcı hata [ayıklama araçlarını kullanarak CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) sorunlarını tanımlayabilirsiniz:
    - Tarayıcıyı açın ve web uygulamasına göz atabilirsiniz.
    - Hata ayıklama konsolunu getirmek için **F12** tuşuna basın.
    - İşlem yeniden üretin ve konsol mesajını gözden geçirin. CORS ihlali kaynak hakkında bir konsol hatası verir.
    - Örneğin, uygulamanız kimlik doğrulaması için login.microsoft.com yeniden yönlendirdiğinde ve erişim belirtecinin süresi dolduğunda bazı CORS sorunları çözülemez. CORS çağrısı başarısız olur. Bu senaryo için geçici bir çözüm, kullanıcının oturumu sırasında süre dolmasını önlemek üzere erişim belirtecinin kullanım süresini uzatmaktır. Bunun nasıl olduğu hakkında daha fazla bilgi için, Microsoft kimlik [platformunda Yapılandırılabilir belirteç yaşam süresine bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **SAML tabanlı çoklu** oturum açma sorunlarını giderme: Karşılaştığınız sorunların çözümlerini bulmak için [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)tabanlı çoklu oturum açma yapılandırılmış uygulamalarda oturum açma sorunlarını denetlemenizi öneririz.
5. **Parola tabanlı çoklu oturum** açma sorunlarını giderme: Karşılaşacak en olası sorunların çözümlerini bulmak için [Azure AD'de](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)parola tabanlı çoklu oturum açma sorunlarını gidermeyi denetlemenizi öneririz.
6. VPN kullanırken bağlantı sorunları için VPN ve diğer bağlantılar üzerinden çoklu oturum [açma (SSO) Wi-Fi bakın.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
