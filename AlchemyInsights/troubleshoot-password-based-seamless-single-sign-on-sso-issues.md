---
title: Parola tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972844"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Parola tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme

Parola tabanlı SSO'nun esaslarını öğrenmek için bkz. SSO ile [parola tabanlı Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Parola tabanlı SSO'yi yapılandırma**

1. [Parola tabanlı çoklu oturum açma ayarlarını yapılandırma](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Bu makale, parola tabanlı SSO seçeneği hakkında daha fazla ayrıntıya girmektedir. Ekley istediğiniz uygulama özel yapılandırma gerektiriyorsa ve parola tabanlı SSO kullanıyorsanız, bu makale tam size göredir.
2. [Uygulama öncesi uygulamalar için parola tabanlı çoklu oturum](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) açma ayarlarını yapılandırma - Uygulama Ara Sunucusu çeşitli çoklu oturum açma modlarını destekler. Parola tabanlı oturum açma, kimlik doğrulaması için kullanıcı adı/parola bileşimi kullanan uygulamalara yöneliktir. Uygulamanız için parola tabanlı oturum açma yapılandırıldığında, kullanıcılarının şirket içi uygulamada bir kez oturum açmaları gerekir. Bundan sonra Azure Active Directory oturum açma bilgilerini depolar ve kullanıcılarınız bilgilerine uzaktan erişene kadar uygulamayı otomatik olarak sağlar.
    - Uygulama Ara Sunucusu ile uygulamanızı zaten yayımladınız ve test ettiysiniz. Bu yoksa, Azure [AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) Uygulama Ara Sunucusu kullanarak uygulamaları yayımlama'daki adımları izleyin ve ardından uygulama öncesi uygulamalar için parola tabanlı SSO yapılandırmanıza devam edin.

Parola tabanlı SSO sorunlarını gidermek için [bkz. Azure AD'de](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) parola tabanlı çoklu oturum açma sorunlarını giderme
