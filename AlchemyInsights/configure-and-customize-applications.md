---
title: Uygulamaları yapılandırma ve özelleştirme
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063712"
---
# <a name="configure-and-customize-applications"></a>Uygulamaları yapılandırma ve özelleştirme

**Uygulamaları Yapılandırma**

1. [Hızlı Başlangıç: Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) kiracısı uygulamanın özelliklerini yapılandırma, uygulamanın bazı özelliklerinin nasıl yapılandırıldığından emin olun.
2. Uygulamalarınızı Azure Active Directory ile tümleştirin, yapılandırmada size yol gösterir [bir](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) öğreticiler koleksiyonu geliştirdik.
3. [Uygulama Ara Sunucusu uygulamasını yapılandırma,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) şirket içi uygulamalarınızı buluta göstermek üzere Azure AD'de Uygulama Ara Sunucusu uygulamasının nasıl yapılandırıldığında anlamanıza yardımcı olur.
4. [PingAccess'i](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)indirin ve uygulamanızı yapılandırma: Ping Kimliği web sitesinde Microsoft Azure AD Uygulama Ara Sunucusu kullanılarak yayımlanan uygulamaları korumak ve PingAccess'in en son sürümünü indirmek için Azure AD için *PingAccess'i* yapılandırma yönergelerini izleyin.

**Hatalı yapılandırılmış Uygulama (AADSTS650056) Hataları**

1. Uygulamaya, uygulama sahibi tarafından sağlanan oturum açma adresiyle erişirken emin olun. Başka bir anlama gelir; uygulamada normal işlemiyle oturum açabilirsiniz. Çoğu durumda bu otomatik olarak doğal bir şekilde çözülecek. Bu gönderi, sorunu gidermenize ve çözmenize yardımcı olabilir.
2. **Uygulamanın sahibi kuruluşsa (bu,** uygulama kaydının kuruluşta olduğu anlamına gelir):
    - En azından `User.Read` Microsoft Graph'in izninin `openid` ekleniyor olması **önerilir.**
    - Uygulamanın ve tüm izinlerinin onaylı olduğundan emin olun. API İzinleri içinde Uygulama kaydının **Durum** sütununa bakarak bunu **doğruabilirsiniz.**
    - Bazı senaryolarda, uygulama üçüncü taraf olabilir, ancak bu uygulama kuruluşta kaydedilmiş olabilir. Bu uygulamanın Uygulama kayıtlarında listelenmiş olup olmadığını onaylayın (Kurumsal uygulamalar değil).
    - Bu hata iletisini görmeye devam edersiniz. Ardından, 4. adımda açıklanan izin **URL'sini oluşturmanız gerekiyor olabilir.**
3. **Organizasyonun sahibi siz değilseniz ve bunu üçüncü taraf bir uygulama olarak kullanıyorsanız:**
    - Genel/Şirket yöneticisiyseniz, izin ekranına bakabilirsiniz. "Organizasyonun adına **izin" kutusunu işaretle işaretleyenin.**
    - İzin ekranı görmüyorsanız Kurumsal uygulamasını silin ve yeniden deneyin.
    - Bu hata iletisini görmeye devam edersiniz. Ardından, 4. adımda açıklanan izin **URL'sini oluşturmanız gerekiyor olabilir.**
4. Kullanılacak izin URL'sini el ile oluşturma: Uygulama belirli bir kaynağa erişmek üzere tasarlanmışsa, Azure portaldan İzin düğmelerini kullanamıyorsanız, kendi izin URL'nizi el ile oluşturmalı ve bunu kullanmalısınız.
    - Uygulamayı sahibinden ve `{App-Id}` `{App-Uri-Id}` sahibinden alırsiniz. `{Tenant-Id}` kiracı tanımlayıcınız olur. Bu, ya sizin `yourdomain.onmicrosoft.com` dizin kimliğiniz olur.
    - Uygulama kaynak için kendisine erişiyorsa, `{App-Id}` ve `{App-Uri-Id}` aynı olacak.
5. Daha fazla bilgi için [BKZ. SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)tabanlı çoklu oturum açma yapılandırılmış uygulamalarda oturum açma sorunları.

**Uygulamaları Özelleştirme**

- [Kuruluş Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) oturum açma sayfasına markalama ekleyin: Azure Active Directory (Azure AD) oturum açma sayfalarınıza tutarlı bir genel görünüm sağlamak için kuruluş logosunu ve özel renk düzenlerini kullanın.
- [Azure Active Directory portalını kullanarak özel etki alanı](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) adınızı ekleyin- Her yeni Azure AD kiracısı, bir ilk etki alanı adıyla gelir. İlk etki alanı adını değiştiremez veya silemezsiniz, ancak kuruluş adlarını eklersiniz. Özel etki alanı adları eklemek, kullanıcılarınıza tanıdık kullanıcı adları oluşturmanıza yardımcı olur.
