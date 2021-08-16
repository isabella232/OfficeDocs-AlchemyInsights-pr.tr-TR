---
title: Sorunsuz SSO'nun şirket içi uygulamalarıma tümleştirme sorunları
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028312"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Sorunsuz SSO'nun şirket içi uygulamalarıma tümleştirme sorunları

Sorunsuz SSO'nun şirket içi uygulamalarla tümleştirmeyle ilgili sorunları gidermek için şunları yapın:

**Önerilen adımlar**

1. Şirket içi bir **uygulamayı** Uygulama Ara Sunucusu üzerinden çoklu oturum açma için yapılandırmak için bkz. Uygulama Ara Sunucusu ile çoklu oturum açma için [parola kasasını açma.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Uygulama Ara Sunucusu sorunlarını** giderme: Uygulama Ara Sunucusu bağlayıcılarının doğru yapılandırıldığından emin olmak için sorun giderme akışı, Uygulama [Ara](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Sunucusu Bağlayıcısı sorunlarını Ayıklama konularını gözden geçirerek başlamanız önerilir. Uygulamaya bağlanma konusunda hala sorun yaşıyorsanız, Uygulama Ara Sunucusu uygulama sorunlarını ayıklama 'daki [sorun giderme adımlarını izleyin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Aşağıdaki tarayıcı hata ayıklama araçlarını kullanarak [CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) sorunlarını tanımlayabilirsiniz:
    1. Tarayıcıyı açın ve web uygulamasına göz atabilirsiniz.
    1. Hata ayıklama konsolunu getirmek için **F12** tuşuna basın.
    1. Işlemi yeniden oluşturmaya çalışarak konsol mesajını gözden geçirebilirsiniz. CORS ihlali kaynak hakkında bir konsol hatası üretir.
    1. Bazı CORS sorunları, örneğin uygulamanın kimlik doğrulaması için login.microsoftonline.com yeniden yönlendirmesi ve erişim belirtecinin süresi dolması gibi sorunları çözemez. CorS çağrısı başarısız olur. Bu senaryo için geçici bir çözüm, kullanıcının oturumu sırasında süresi dolmasını önlemek üzere erişim belirtecin kullanım süresini uzatmaktır. Bunun nasıl olduğu hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)Microsoft kimlik platformu.

**Önerilen belgeler**

- [Uygulama Ara Sunucusu uygulamasında çoklu oturum açma nasıl yapılandırılır](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Uygulama Ara Sunucusu ile şirket içi uygulamalar için SAML çoklu oturum açma](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Uygulama Ara Sunucusu CORS Azure Active Directory sorunlarını anlama ve çözme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Uygulama Ara Sunucusu için Kerberos kısıtlanmış temsilci yapılandırmalarında sorun giderme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)