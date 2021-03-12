---
title: Parola Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714890"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Parola Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme

Parola tabanlı SSO'nun temellerini öğrenmek için Azure [Active Directory ile Parola tabanlı kimlik doğrulamasına bakın.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Parola tabanlı SSO'nun yapılandırılması**

1. [Parola tabanlı çoklu oturum açma ayarlarını yapılandırma](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Bu makale, parola tabanlı SSO seçeneği hakkında daha fazla ayrıntıya gider. Ekley istediğiniz uygulama özel yapılandırma gerektiriyorsa ve parola tabanlı SSO kullanıyorsanız, bu makale tam size göredir.
2. [Uygulama öncesi uygulamalar için parola tabanlı çoklu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) oturum açma ayarlarını yapılandırma - Uygulama Ara Sunucusu çeşitli çoklu oturum açma modlarını destekler. Parola tabanlı oturum açma, kimlik doğrulaması için kullanıcı adı/parola bileşimi kullanan uygulamalara yöneliktir. Uygulamanız için parola tabanlı oturum açma yapılandırıldığında, kullanıcılarının şirket içi uygulamada bir kez oturum açmaları gerekir. Bundan sonra, Azure Active Directory oturum açma bilgilerini depolar ve kullanıcılarınız uzaktan erişse uygulamaya otomatik olarak sağlar.
    - Uygulama Ara Sunucusu ile uygulamanızı zaten yayımlanmış ve test edilmiş olması gerekir. Yoksa, Azure AD [Application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) Proxy'lerini kullanarak Uygulamaları yayımla'daki adımları izleyin ve ardından uygulama öncesi uygulamalar için parola tabanlı SSO yapılandırmanıza devam edin.

Parola tabanlı SSO sorunlarını gidermek için Bkz. [Azure AD'de](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) parola tabanlı çoklu oturum açma sorunlarını giderme
