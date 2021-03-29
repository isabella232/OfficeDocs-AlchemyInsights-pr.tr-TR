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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402287"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Sorunsuz Çoklu Oturum Açma(SSO) Yapılandırma

**Uygulamaları Yapılandırma**

1. Değerleri uygulama satıcısından alısınız. Değerleri el ile girebilirsiniz veya alanların değerini ayıklamak için bir meta veri dosyası karşıya yükleyebilirsiniz.
2. Birçok uygulama Azure AD ile çalışmak için önceden yapılandırılmış. Bu uygulamalar, Azure AD kiracınıza uygulama eklerken göz atabilirsiniz uygulama galerisinde listelenir. Hızlı [başlangıç serisi,](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) bu işlemde size yol sağlar.
3. Galeri olmayan bir uygulama oluşturmak için , **+** Kendi Uygulamanızı Oluştur düğmesine tıklayabilirsiniz ve Uygulamanıza bir ad veebilirsiniz.
    - Varsayılan olarak, Galeri dışı **uygulamalar** için doğru seçenek olan galeride bulmanız gerekilmeyen diğer tüm uygulamaları tümleştir'i seçer.
    - Uygulamanın adını **verdikten** sonra Oluştur'a bir kez olduktan sonra, yeni bir Galeri Dışı Kurumsal Uygulama oluşturacak.
    - Daha sonra, bu **uygulamanın** yönetimi  altında Çoklu Oturum Açma'ya gidin ve ortamınıza uygulamayı farklı teknikler de ebilirsiniz.

**Belirli bir uygulama için Sorunsuz SSO'nun yapılandırılması**

Galeride yer alan uygulamalar için ayrıntılı, adım adım yönergeleri bulabilirsiniz. Adımlara erişmek için, SaaS uygulama yapılandırma öğreticileri'nde tüm uygulama [yapılandırma öğreticilerinin listesine göz atabilirsiniz.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML tabanlı SSO'u yapılandırma**

1. [Hızlı Başlangıç: Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)kiracınıza bir uygulama için SAML tabanlı çoklu oturum açma (SSO) ayarlama.
2. Çoklu oturum açma için SAML tabanlı seçenek hakkında daha fazla bilgi edinmek için bkz. [SAML tabanlı çoklu oturum açma hakkında daha fazla bilgi.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Azure Active Directory'nin (Azure AD Sign-On) Çoklu Oturum Açma (SSO) için desteklediği SAML 2.0 kimlik doğrulama istekleri ve yanıtları hakkında bilgi edinmek için bkz. Tek Sign-On [SAML protokolü.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Microsoft Graph API'sini kullanarak Azure Active Directory'de (Azure AD) uygulamanız için SAML tabanlı çoklu oturum açma (SSO) oluşturma ve yapılandırma hakkında bilgi edinmek için bkz. Microsoft Graph API'sini kullanarak uygulamanız için [SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)tabanlı çoklu oturum açma yapılandırma.
5. Azure AD'nin SAML protokolünü nasıl kullandığını öğrenmek için bkz. [Microsoft kimlik platformu SAML protokolünü nasıl kullanır?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Belirteçleri ve talepleri yapılandırma**

1. [Kurumsal uygulamalar için SAML belirtecinde verilen talepler nasıl özelleştirilebilir?](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. PowerShell kullanarak talep yapılandırmayı öğrenmek için bkz. Kiracıdaki belirli bir uygulamanın belirteçleri içinde yer alan talepleri özelleştirme [(Önizleme)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. İsteğe bağlı talepler yapılandırmayı öğrenmek için bkz. [Uygulamanıza isteğe bağlı talepler sağlama.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Belirteç talebinde uygulamalara kullanıcı verileri gönderirken dizin şema uzantısı özniteliklerini kullanmayı öğrenmek için, bkz. Taleplerde dizin [şema uzantısı özniteliklerini kullanma.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Belirteç yaşam sürelerini yapılandırmayı öğrenmek için, Microsoft kimlik platformunda [(önizleme) Yapılandırılabilir belirteç yaşam süresine bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Belirteç yaşam süresi ilkelerini (önizleme)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) yapılandırma - Bu makalede, belirteç yaşam süresi için yeni kurallar uygulamanıza yardımcı olacak genel bir ilke senaryosunu adım adım takip ederiz. Örnekte, kullanıcıların web uygulamanıza daha sık kimlik doğrulaması yapmalarını gerektiren bir ilkenin nasıl oluşturulanı öğrenirsiniz.

**SSO Yapılandırması sorunlarını giderme**

- Azure Active Directory Sorunsuz Çoklu Oturum Açma (Sorunsuz SSO) hakkında sık sorulan Sign-On, Azure Active Directory Sorunsuz Çoklu Oturum [Açma: Sık sorulan sorular.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Azure Active Directory (Azure AD) Sorunsuz Çoklu Oturum Açma (Sorunsuz SSO) ile ilgili sık karşılaşılan sorunlar hakkında Sign-On için [bkz. Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)Sorunsuz Çoklu Oturum Açma sorunlarını giderme.
