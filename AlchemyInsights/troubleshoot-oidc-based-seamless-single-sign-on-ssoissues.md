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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747134"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC Tabanlı Sorunsuz Çoklu Oturum Açma (SSO) sorunlarını giderme

- Azure kiracınıza OIDC tabanlı bir uygulama ekleme hakkında bilgi edinmek için [bkz. Hızlı Başlangıç: Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)kiracınıza bir uygulama için OIDC tabanlı çoklu oturum açma (SSO) ayarlama.
- Çoklu oturum açma uygulamak için OpenID Connect standardını kullanan uygulamalar hakkında daha fazla ayrıntı için bkz. [OIDC tabanlı çoklu oturum açmayı anlama.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- HTTP isteklerini doğrudan göndererek ve işerek kodunuzu yazmayı ya da açık kaynak kitaplıklarımızı kullanmak yerine üçüncü taraf bir açık kaynak kitaplığı kullanmayı seçmeniz durumunda, Microsoft kimlik [platformunda OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)ve OpenID Connect protokollerine bakın.

**Protokoller**

1. [Microsoft kimlik platformu](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) ve dolaylı grant flow - Dolaylı iznin tanımlama özelliği, belirteçlerin (kimlik belirteçleri veya erişim belirteçleri) /token uç noktası yerine doğrudan /authorize uç noktasının üzerinden döndürülmedir. Bu genellikle "karma akış" olarak adlandırılan yetkilendirme kodu akışının bir parçası olarak **kullanılır; yetkilendirme** koduyla birlikte /yetki isteğinde kimlik belirteci alınır. Bu makalede, Azure AD'den belirteçleri talep etmek için doğrudan uygulamanıza yönelik protokole karşı nasıl programla ilgili açıklanmıştır.
2. [Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) yetkilendirme kodu akışı - OAuth 2.0 yetkilendirme kodu izni, web API'leri gibi korumalı kaynaklara erişmek için bir cihaza yüklenmiş olan uygulamalarda kullanılabilir. OAuth 2.0'ın Microsoft kimlik platformu uygulamasını kullanarak, mobil ve masaüstü uygulamalarınıza oturum açma **ve API erişimi ebilirsiniz.** Bu makalede, herhangi bir dili kullanarak uygulamanıza yönelik protokole karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
3. [Microsoft kimlik platformu ve OpenID Connect protokolü](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Microsoft kimlik platformunun OpenID Connect uygulamasını kullanarak uygulamalarınıza oturum açma ve API erişimi ebilirsiniz. Bu makalede, bunun dilden bağımsız olarak nasıl yerine konulları açıklanmıştır ve Microsoft açık kaynak kitaplıklarını kullanmadan HTTP iletileri gönderme **ve alma açıklanmıştır.**
4. Microsoft kimlik platformu ve OAuth 2.0 istemci kimlik bilgileri akışı - Bir uygulamanın kimliğini kullanarak web'de barındırılan kaynaklara erişmek için RFC 6749'da (bazen iki okunaklı **OAuth** olarak da anlanan) belirtilen [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgilerini kullanabilirsiniz. Bu tür bir bağış, genellikle kullanıcıyla hemen etkileşim olmadan arka planda çalışması gereken sunucudan sunucuya etkileşimlerde kullanılır. Bu tür uygulamalar genellikle **daemons** veya hizmet hesapları **olarak adlandırılır.** Bu makalede, uygulamanın protokole karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
