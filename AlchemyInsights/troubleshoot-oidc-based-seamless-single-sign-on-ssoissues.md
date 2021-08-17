---
title: OIDC Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105804"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme

- Azure kiracınıza OIDC tabanlı bir uygulama ekleme hakkında bilgi edinmek için bkz. Hızlı Başlangıç: Azure Active Directory (Azure AD) kiracınıza bir uygulama için OIDC tabanlı çoklu oturum açma [(SSO) ayarlama.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Çoklu oturum açma uygulamak için OpenID Bağlan standardını kullanan uygulamalar hakkında daha fazla ayrıntı için bkz. [OIDC tabanlı çoklu oturum](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)açma hakkında bilgi edinin.
- Kodunuzu, HTTP isteklerini doğrudan göndererek ve işerek yazmayı ya da açık kaynak kitaplıklardan birini kullanmak yerine üçüncü taraf bir açık kaynak kitaplığı kullanarak yazmanız durumunda bilgi için, dosya üzerinde [OAuth 2.0 ve OpenID Bağlan protokollerine Microsoft kimlik platformu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokoller**

1. [Microsoft kimlik platformu](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) ve örtülü grant akışı - Dolaylı iznin tanımlama özelliği, belirteçlerin (kimlik belirteçleri veya erişim belirteçleri) /token uç noktası yerine doğrudan /authorize uç noktalarından döndürül vermesidir. Bu genellikle "karma akış" olarak adlandırılan yetkilendirme kodu akışının bir parçası olarak kullanılır; yetkilendirme koduyla birlikte /authorize isteğinde kimlik belirteci **alınır.** Bu makalede, Azure AD'den belirteç talep etmek için uygulamanıza doğrudan protokol üzerinden nasıl programla ilgili olduğu açıklanmıştır.
2. [Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) yetkilendirme kodu akışı - OAuth 2.0 yetkilendirme kodu izni, web API'leri gibi korunan kaynaklara erişmek için bir cihaza yüklenmiş olan uygulamalarda kullanılabilir. OAuth 2.0'ın Microsoft kimlik platformu uygulamasını kullanarak, mobil ve masaüstü uygulamalarınıza oturum açma **ve API erişimi eklersiniz.** Bu makalede, herhangi bir dili kullanarak uygulamanıza yönelik protokole karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
3. [Microsoft kimlik platformu ve OpenID Bağlan protokolü](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Microsoft kimlik platformu'nin OpenID Bağlan uygulamasını kullanıyorken, uygulamalarınıza oturum açma ve API erişimi ebilirsiniz. Bu makalede bunun dilden bağımsız olarak nasıl yerine tabi olduğu açıklanmıştır ve Microsoft açık kaynak kitaplıklarını kullanmadan HTTP iletileri gönderme **ve alma açıklanmıştır.**
4. [Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgileri akışı - Bir uygulamanın kimliğini kullanarak web'de barındırılan kaynaklara erişmek için RFC 6749'da belirtilen veya bazen iki okunaklı OAuth olarak da adlandırılan **OAuth** 2.0 istemci kimlik bilgilerini kullanabilirsiniz. Bu tür bir verim, genellikle kullanıcıyla acil etkileşim olmadan arka planda çalışması gereken sunucudan sunucuya etkileşimlerde kullanılır. Bu tür uygulamalar genellikle **daemons veya** hizmet **hesapları olarak adlandırılır.** Bu makalede, uygulamanın protokolüne karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
