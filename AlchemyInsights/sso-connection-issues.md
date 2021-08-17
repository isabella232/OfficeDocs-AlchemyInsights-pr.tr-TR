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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084366"
---
# <a name="sso-connection-issues"></a>SSO Bağlantı Sorunları

1. Hızlı [Başlangıç: Başvuru kılavuzu için özellikleri yapılandırarak](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) uygulamayı yapılandırma adımlarını izleyin.
2. Seçtiğiniz uygulama ve Çoklu [oturum açma seçeneğine bağlı](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) olarak, aşağıdaki uygun yönergeleri izleyin:
    - **SAML** **tabanlı çoklu** oturum açma için şirket içi bir uygulama yapılandırmak için bkz. Uygulama Ara Sunucusu ile şirket içi uygulamalar için [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)çoklu oturum açma.
    - Parola tabanlı **çoklu oturum açma** için bir bulut uygulamasını yapılandırmak için **bkz.** [Parola çoklu oturum açmayı yapılandırma.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Şirket içi bir **uygulamayı** Uygulama Ara Sunucusu üzerinden çoklu oturum açma için yapılandırmak için bkz. Uygulama Ara Sunucusu ile çoklu oturum açma için [parola kasasını açma.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Uygulama Ara Sunucusu sorunlarını giderme:** Uygulama Ara Sunucusu bağlayıcılarının doğru yapılandırıldığından emin olmak için sorun giderme akışını, Uygulama [Ara](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Sunucusu Bağlayıcısı sorunlarını Ayıklama'yi gözden geçirerek başlamanız önerilir. Uygulamaya bağlanma konusunda hala sorun yaşıyorsanız, Uygulama Ara Sunucusu uygulaması sorunlarını Ayıklama 'daki sorun giderme [akışını izleyin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Tarayıcı hata [ayıklama araçlarını kullanarak CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) sorunlarını tanımlayabilirsiniz:
    - Tarayıcıyı açın ve web uygulamasına göz atabilirsiniz.
    - Hata ayıklama konsolunu getirmek için **F12** tuşuna basın.
    - Işlemi yeniden oluşturmaya çalışarak konsol mesajını gözden geçirebilirsiniz. CORS ihlali kaynak hakkında bir konsol hatası üretir.
    - Bazı CORS sorunları, örneğin uygulamanın kimlik doğrulaması için login.microsoft.com yeniden yönlendirmesi ve erişim belirtecinin süresi dolması gibi sorunları çözemez. CorS çağrısı başarısız olur. Bu senaryo için geçici bir çözüm, kullanıcının oturumu sırasında süresi dolmasını önlemek üzere erişim belirtecin kullanım süresini uzatmaktır. Bunun nasıl olduğu hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)Microsoft kimlik platformu.
4. **SAML** tabanlı çoklu oturum açma sorunlarını giderme : En sık karşılaşacakları sorunların çözümlerini bulmak [için, SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)tabanlı çoklu oturum açma yapılandırılmış uygulamalarda oturum açma sorunları denetlenmenizi öneririz.
5. **Parola tabanlı çoklu oturum açma sorunlarını giderme:** En sık karşılaşacakları sorunların çözümlerini bulmak için [Azure AD'de](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)parola tabanlı çoklu oturum açma sorunlarını giderme'ye göz atmanizi öneririz.
6. VPN kullanırken bağlantı sorunları için bkz. VPN ve güvenlik bağlantıları üzerinden çoklu oturum [açma (SSO) Wi-Fi.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
