---
title: OAuth 2.0 ve OpenID Connect protokolleri sorunlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037695"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2.0 ve OpenID Connect protokolleri sorunlarını giderme

OAuth 2.0 ve OpenID Connect sorunlarını çözmek için, aşağıdaki önerilen adımları uygulayın:

OAuth 2.0 ve OpenID Connect protokolleri ile ilgili yapılandırma ve sorun gidermeyle ilgili aşağıdaki makalelere bakın:

- [Microsoft kimlik platformu ve OAuth 2.0 yetkilendirme](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) kodu akışı - Bu makalede, herhangi bir dili kullanarak uygulamanıza doğrudan kod desteği **(PKCE)** akışına karşı nasıl programlaynız açıklanmıştır.
- [Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgileri akışı - Bu makalede, uygulamanın istemci kimlik bilgileri akışına karşı doğrudan nasıl **programlanacakları** açıklanmıştır.
- [Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) Kaynak Sahibi Parola Kimlik Bilgileri - Bu makalede, uygulamanın **ROPC** akışına karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
    - Microsoft kimlik platformu yalnızca Azure AD kiracıları için ROPC'i destekler, kişisel hesaplar için desteklemez. Bu, kiracıya özgü bir uç nokta (veya kuruluşlar **uç noktası) https://login.microsoftonline.com/{TenantId_or_Name})** **kullanmanız gerektiğini belirtir.**
    - Azure AD kiracısına davet edilen kişisel hesaplar ROPC'yi kullanamayabilirsiniz.
    - Parolasız hesaplar ROPC aracılığıyla oturum açmaz. Bu senaryo için, bunun yerine uygulamanız için farklı bir akış kullanmanızı öneririz.
    - Kullanıcıların uygulamada oturum [açmak için Multi-Factor Authentication (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) kullanmaları gerekirse, bunlar engellenir.
    - ROPC, karma kimlik [](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) federasyonu senaryolarında (örneğin, şirket içi hesapların kimliğini doğrulamak için kullanılan Azure AD ve ADFS) desteklenmiyor. Kullanıcılar şirket içi kimlik sağlayıcısına tam sayfa yeniden yönlendirildiyseniz, Azure AD kullanıcı adını ve parolayı bu kimlik sağlayıcısına karşı test edememektedir. [Bununla birlikte, ropc](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) ile geçişli kimlik doğrulaması da desteklenir.
    - Karma kimlik federasyonu senaryosu için bir özel durum şu olabilir: **AllowCloudPasswordValidation** değeri **TRUE** olarak ayarlanmış Ev Realm Discovery ilkesi, şirket içi parola bulutla eşitlenirken ŞIRKET içi kullanıcılar için ROPC akışının çalışmasına olanak sağlar. Daha fazla bilgi için eski [uygulamalar için federasyon kullanıcılarının doğrudan ROPC kimlik doğrulamasını etkinleştirme](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft kimlik platformu ve OAuth 2.0 Adına-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - Bu makalede, uygulamanın adına **(OBO)** akışına karşı nasıl doğrudan programla ilgili olduğu açıklanmıştır.
- [Microsoft kimlik platformu ve OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) protokolü - Bu makalede OpenID Connect protokolünün dilden bağımsız olarak nasıl uygulandığını gösterir ve Microsoft açık kaynak kitaplıklarını kullanmadan HTTP iletilerinin nasıl gönder ve al uygulandığını açıklar.

**Erişim Belirteçleri**

[Microsoft kimlik platformu erişim belirteçleri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API'nizin bir erişim belirteci içindeki talepleri nasıl doğrulaya ve kullanabileceğini öğrenin. Bu makaledeki tüm belgeler, not edildi dışındaki yalnızca kayıtlı API'ler için verilen belirteçlere uygulanır. Microsoft'a ait API'ler için verilen belirteçler için geçerli değildir ve bu belirteçler, Microsoft kimlik platformunun sizin oluşturtuz bir API için belirteçleri nasıl çıkartır olacağını doğrulamak için kullanılamaz.

**Uygulama Yapılandırması**

[Yeniden Yönlendirme URI'si (yanıt URL'si)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) kısıtlamaları ve sınırlamaları - Yeniden Yönlendirme URI'nizi (yanıt URL'si) yapılandırmayı öğrenin. Yeniden yönlendirme URI'si veya yanıt URL'si, uygulama başarıyla yetkilendirilip bir yetkilendirme kodu veya erişim belirteci verildiktan sonra yetkilendirme sunucusunun kullanıcıya gönderdiği konumdur. Yetkilendirme sunucusu kodu veya belirteci yeniden yönlendirme URI'sini gönderir; bu nedenle, uygulama kayıt işleminin bir parçası olarak doğru konumu kaydetmeniz önemlidir.

**Uygulama Hazırlama**

[Öğretici: SCIM uç noktası](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) için sağlamayı geliştirme ve planlama - Bu makalede, SCIM uç noktasının nasıl inşa edilmiş ve AAD sağlama hizmetiyle tümleştiriliği açıklanmıştır.


