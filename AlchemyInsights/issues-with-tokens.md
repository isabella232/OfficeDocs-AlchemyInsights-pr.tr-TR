---
title: Belirteçlerle ilgili sorunlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917214"
---
# <a name="issues-with-tokens"></a>Belirteçlerle ilgili sorunlar

Belirteçleriyle ilgili sorunları yönetmek için aşağıdaki adımları gerçekleştirebilirsiniz:

1. Microsoft Identity platform tarafından verilen bir erişim, KIMLIK veya SAML belirtecinin yaşam süresini belirtebilirsiniz. Kuruluşunuzdaki tüm uygulamalar için, birden çok kiracı (çok kuruluş) uygulaması veya kuruluşunuzdaki belirli bir hizmet sorumlusu için belirteç ömürleri ayarlayabilirsiniz. Daha fazla bilgi için [Microsoft Identity platform (Preview) ' da yapılandırılabilir belirteç ömürleri](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)konusuna bakın.
2. Access belirteçleri, istemcilerin korumalı Web API 'Lerini güvenli bir şekilde aramasını sağlar ve kimlik doğrulama ve yetkilendirmeyi gerçekleştirmek için Web API 'Leri tarafından kullanılır. OAuth belirtiminde olduğu gibi, Access belirteçleri küme biçimi olmayan opak dizelerdir-bazı kimlik sağlayıcıları (IDPs), diğerleri şifreli blob kullanırlar. Microsoft Identity platform, belirteci kabul eden API yapılandırmasına bağlı olarak çeşitli erişim belirteci biçimleri kullanır. API 'unuzun bir erişim belirtecinin içindeki talepleri nasıl doğrulayabildiğini ve kullanabileceğinizi öğrenmek için [Microsoft Identity platform erişim belirteçleri](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)bölümüne bakın.
3. Microsoft kimlik doğrulama kitaplığı (MSAL) farklı uygulama senaryolarında kullanılmak üzere çeşitli kimlik doğrulama akışlarını destekler. Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)
4. OAuth 2,0 yetkilendirme kodu izni, Web API 'Leri gibi korumalı kaynaklara erişim kazanmak için cihazda yüklü olan uygulamalarda kullanılabilir. OAuth 2,0 Microsoft Identity platform uygulamasını kullanarak, cep telefonu ve Masaüstü uygulamalarınıza oturum açma ve API erişimi ekleyebilirsiniz. Herhangi bir dil kullanarak doğrudan uygulamanızdaki protokole nasıl programlayabileceğiniz hakkında [Microsoft Identity platform ve OAuth 2,0 yetkilendirme kodu akışını](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) görün.
5. OpenID Connect (OıDC), bir kullanıcıya güvenli bir şekilde oturum açmak için kullanabileceğiniz, OAuth 2,0 üzerinde oluşturulmuş bir kimlik doğrulama protokolüdür. OpenID Connect 'in Microsoft Identity platform uç noktasının uygulamasını kullandığınızda, uygulamalarınıza oturum açma ve API erişimi ekleyebilirsiniz. [Microsoft Identity platform ve OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) , bu dilden bağımsız olarak nasıl yapılacağını ve Microsoft açık kaynak KITAPLıKLARıNı kullanmadan http iletilerini nasıl gönderip alacağınızı açıklar.
    - UserInfo uç noktası OıDC standardının bir parçasıdır ve kimliği doğrulanmış kullanıcıyla ilgili talepleri döndürmek için tasarlanmıştır. Daha fazla bilgi için [Microsoft Identity platform UserInfo uç noktasına](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)bakın.
    - [Azure AD ve OpenID Connect örneği kullanılarak bir Web uygulamasında bir Web API 'Sinin çağrılması](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) , OpenID Connect protokolünü kullanarak oturum açma IÇIN Azure AD 'yi kullanan bir MVC web uygulamasının nasıl oluşturulduğunu gösterir ve ardından OAuth 2,0 aracılığıyla alınan belirteçleri kullanarak oturum açan kullanıcının kimliği altındaki BIR Web API 'sini arar. Bu örnekte OpenID Connect ASP .net 'in ara yazılımı ve ADAL .net kullanılmaktadır.
6. [Uygulamayı bir Web API 'si sergilemek Için yapılandırma](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -bu hızlı başlangıç sırasında, Microsoft Identity platformuyla BIR Web API kaydettirir ve örnek bir kapsam ekleyerek istemci uygulamalarına açarsınız. Web API 'sini kaydederek ve kapsamlar aracılığıyla kullanıma sunarak, istemcilere, yetkili kullanıcılara ve API 'ınıza erişen istemci uygulamalarına izinler temelinde erişim sağlayabilirsiniz.
7. Azure Active Directory B2C 'de (Azure AD B2C), kaynak sahibi parolası kimlik bilgileri (ROPC) akışı, bir OAuth standart kimlik doğrulama akışdır. Bu akışta, bağlı taraf olarak da bilinen bir uygulama, belirteçler için geçerli kimlik bilgilerini değişimler. Kimlik bilgileri bir kullanıcı KIMLIĞI ve parola içerir. Döndürülen belirteçler bir KIMLIK belirteci, erişim belirteci ve yenileme belirteci. Daha fazla bilgi için, [Azure Active DIRECTORY B2C 'de kaynak sahibi parolası kimlik bilgileri akışını ayarlama](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)bölümüne bakın. 

