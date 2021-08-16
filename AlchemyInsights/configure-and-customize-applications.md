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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045008"
---
# <a name="configure-and-customize-applications"></a>Uygulamaları yapılandırma ve özelleştirme

**Uygulamaları Yapılandırma**

1. [Hızlı Başlangıç: Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) kiracısı uygulamanın özelliklerini yapılandırma, uygulamanın bazı özelliklerinin nasıl yapılandırıldığından emin olun.
2. Uygulamalarınızı Azure Active Directory tümleştirin yardımcı olmak için, [yapılandırmada size yol](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) geliştiren bir öğreticiler koleksiyonu geliştirdik.
3. [Uygulama Ara Sunucusu uygulamasını yapılandırma,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) Azure AD içinde bir Uygulama Ara Sunucusu uygulamasını şirket içi uygulamalarınızı buluta açık olacak şekilde yapılandırmanızı anlamanıza yardımcı olur.
4. [PingAccess'i](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)indirin ve uygulamanızı yapılandırma : Ping Kimliği web sitesinde Microsoft Azure AD Uygulama Ara Sunucusu kullanarak yayımlanan uygulamaları korumak ve PingAccess'in en son sürümünü indirmek için Azure AD için *PingAccess'i* yapılandırma yönergelerini izleyin.

**Hatalı Yapılandırılmış Uygulama (AADSTS650056) Hataları**

1. Uygulamaya, uygulama sahibi tarafından sağlanan oturum açma adresiyle erişirkenn emin olun. Başka bir anlama gelir; uygulamada normal işlemiyle oturum açabilirsiniz. Çoğu durumda bu otomatik çözüm doğal bir şekilde çözülecek. Bunu çözemezse, bu gönderi sorun gidermeye ve çözmeye yardımcı olabilir.
2. **Uygulamanın kuruluşu size aitse** (uygulama kaydının kurum içinde olduğu anlamına gelir):
    - En azından Microsoft'un `User.Read` izinlerini veya `openid` temsilci olarak Graph öneririz. 
    - Uygulamanın ve tüm izinlerinin onaylı olduğundan emin olun. API İzinleri içinde Uygulama kaydının **Durum** sütununa bakarak bunu **doğruabilirsiniz.**
    - Bazı senaryolarda, uygulama üçüncü taraf olabilir, ancak uygulama kuruluşta kaydedilmiş olabilir. Bu uygulamanın Uygulama kayıtlarında listelenmiş olup olmadığını onaylayın (Enterprise değil).
    - Bu hata iletisini görmeye devam edersiniz. Ardından, 4. adımda açıklanan izin **URL'sini oluşturmanız gerekiyor olabilir.**
3. **If your organization is not the application owner and using it as a third-party application**:
    - Genel/Şirket yöneticisiyseniz, izin ekranına bakabilirsiniz. "Organizasyonun adına **izin" onay kutusunu işaretle işaret olduğundan emin olun.**
    - İzin ekranı görmüyorsanız, Enterprise silin ve yeniden deneyin.
    - Bu hata iletisini görmeye devam edersiniz. Ardından, 4. adımda açıklanan izin **URL'sini oluşturmanız gerekiyor olabilir.**
4. Kullanılacak izin URL'sini el ile oluşturma: Uygulama belirli bir kaynağa erişecek şekilde tasarlanmışsa, Azure portaldan İzin düğmelerini kullanamıyorsanız kendi izin URL'nizi kendiniz oluşturmalı ve bunu kullanmalısınız.
    - Ve uygulamasını sahibinden `{App-Id}` `{App-Uri-Id}` alırsiniz. `{Tenant-Id}` kiracı tanımlayıcınız olur. Bu, ya sizin `yourdomain.onmicrosoft.com` dizin kimliğiniz olur.
    - Uygulama kaynak için kendisine erişiyorsa ve aynı `{App-Id}` `{App-Uri-Id}` olacaksa.
5. Daha fazla bilgi için [bkz. SAML tabanlı](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)çoklu oturum açma yapılandırılmış uygulamalarda oturum açma sorunları .

**Uygulamaları Özelleştir**

- [Kuruluş oturum](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) açma sayfasına Azure Active Directory ekleme - Azure Active Directory (Azure AD) oturum açma sayfalarınıza tutarlı bir genel görünüm sağlamak için kuruluş logosunu ve özel renk düzenlerini kullanın.
- Yeni bir Azure AD [kiracısı olan Azure Active Directory alanı](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) adınızı şu portal aracılığıyla ekleyin: Her yeni Azure AD kiracısı, bir ilk etki alanı adıyla gelir. İlk etki alanı adını değiştiremez veya silemezsiniz, ancak kuruluş adlarını ebilirsiniz. Özel etki alanı adları eklemek, kullanıcılarınıza tanıdık kullanıcı adları oluşturmanıza yardımcı olur.
