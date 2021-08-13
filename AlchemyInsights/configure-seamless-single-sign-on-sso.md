---
title: Sorunsuz Çoklu Oturum Açma (SSO) Yapılandırma
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966057"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Sorunsuz Çoklu Oturum Açma (SSO) Yapılandırma

**Uygulamaları Yapılandırma**

1. Değerleri uygulama satıcısından alısınız. Alanların değerini ayıklamak için değerleri el ile girebilir veya bir meta veri dosyası karşıya yükleyebilirsiniz.
2. Birçok uygulama Azure AD ile çalışmak için önceden yapılandırılmış. Bu uygulamalar, Azure AD kiracınıza uygulama eklerken göz atabilirsiniz uygulamalar galerisinde listelenir. Hızlı [başlangıç serisi,](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) bu süreçte size yol sağlar.
3. Galeri dışı bir uygulama oluşturmak için + Kendi Uygulamanızı oluşturun **düğmesine tıklayabilirsiniz ve** Uygulamanıza bir ad veebilirsiniz.
    - Varsayılan olarak, Galeri dışı **uygulamalar için doğru** seçenek olan galeride bulmanız gerekilmeyen diğer tüm uygulamaları tümleştir'i seçer.
    - Uygulamanın adını **verdikten** sonra Oluştur'a indikten sonra, Uygulama için yeni Bir Galeri dışı Enterprise oluşturması gerekir.
    - Ardından, Bu uygulamanın yönetimi **altında** Çoklu Oturum Açma'ya gidin; bunu ortamınıza uygulamak için farklı teknikler de görebilirsiniz. 

**Belirli bir uygulama için Sorunsuz SSO yapılandırma**

Galeride yer alan uygulamalar için ayrıntılı, adım adım yönergeleri bulabilirsiniz. Adımlara erişmek için SaaS uygulama yapılandırma öğreticileri'nde tüm uygulama yapılandırma [öğreticilerinin listesine göz atabilirsiniz.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML tabanlı SSO'u yapılandırma**

1. Hızlı Başlangıç: Azure Active Directory (Azure AD) kiracısı uygulamanız için SAML tabanlı çoklu oturum açma [(SSO) ayarlama.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Çoklu oturum açma için SAML tabanlı seçenek hakkında daha fazla bilgi edinmek için bkz. [SAML tabanlı çoklu oturum](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)açma hakkında bilgi.
3. Çoklu Kimlik Doğrulaması (SSO Sign-On) için Azure Active Directory(Azure AD) tarafından destekleyen SAML 2.0 kimlik doğrulama istekleri ve yanıtları hakkında bilgi edinmek için bkz. Tek kimlik Sign-On [SAML protokolü.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Microsoft Graph API'sini kullanarak Azure Active Directory'de (Azure AD) uygulamanız için SAML tabanlı çoklu oturum açma (SSO) oluşturma ve yapılandırma hakkında bilgi edinmek için bkz. Microsoft Graph API'sini kullanarak uygulamanız için [SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)tabanlı çoklu oturum açmayı yapılandırma.
5. Azure AD'nin SAML protokolünü nasıl kullandığını öğrenmek için bkz. [Microsoft kimlik platformu, SAML protokolünü nasıl kullanır.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Belirteçleri ve Talepleri Yapılandırma**

1. [Kurumsal uygulamalar için SAML belirtecinde verilen talepler nasıl özelleştirilebilir.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. PowerShell kullanarak talepleri yapılandırmayı öğrenmek için bkz. Nasıl [yapılandırılır: Kiracıdaki](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)belirli bir uygulama için belirteçlerde talepleri özelleştirme (Önizleme) .
3. İsteğe bağlı talepler yapılandırmayı öğrenmek için [bkz. Nasıl yapılan: Uygulamanıza isteğe bağlı talepler sağlama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Belirteç iddialarında uygulamalara kullanıcı verileri gönderirken dizin şema uzantısı özniteliklerini kullanmayı öğrenmek için bkz. Taleplerde dizin [şema uzantısı özniteliklerini kullanma](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Belirteç yaşam sürelerini yapılandırmayı öğrenmek için bkz. Son (önizleme) Microsoft kimlik platformu [kullanım ömrü.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Belirteç yaşam süresi ilkelerini (önizleme)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) yapılandırma - Bu makalede, belirteç yaşam süresi için yeni kurallar uygulamanıza yardımcı olacak genel bir ilke senaryosu üzerinden geçeceğiz. Örnekte, kullanıcıların web uygulamanıza daha sık kimlik doğrulaması yapmalarını gerektiren bir ilke oluşturma hakkında bilgi edinebilirsiniz.

**SSO Yapılandırması sorunlarını giderme**

- Sorunsuz Çoklu Oturum Açma (Sorunsuz Azure Active Directory (Sorunsuz SSO) Sign-On Azure Active Directory hakkında sık sorulan sorular için bkz. Sorunsuz Çoklu Azure Active Directory [Açma: Sık sorulan sorular](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Sorunsuz Çoklu Oturum Açma (Azure AD Sign-On) (Azure AD) Azure Active Directory (Sorunsuz SSO) ile ilgili yaygın Azure Active Directory sorunları giderme için bkz. Sorunsuz Çoklu Azure Active Directory açma ile [ilgili sorunları giderme.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
