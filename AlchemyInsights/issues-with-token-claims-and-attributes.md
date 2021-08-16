---
title: Belirteç talebi ve öznitelikleriyle ilgili sorunlar
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012904"
---
# <a name="issues-with-token-claims-and-attributes"></a>Belirteç talebi ve öznitelikleriyle ilgili sorunlar

**Belirteç iddialarını güncelleştirme, yapılandırma veya kaldırma**

1. Etki Azure Active Directory (Azure AD) kullanarak, [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) uygulamayı yetkilendirdikten sonra size verilen yanıt belirtecinde rol talebi için talep türünü özelleştirebilirsiniz.
2. Uygulama geliştiriciler, uygulamalarına gönderilen belirteçlerde hangi talepte yer almak istemedilerini belirtmek için Azure AD uygulamalarında isteğe bağlı talepler kullanabilir. Daha fazla bilgi için [bkz. Uygulamanıza isteğe bağlı talepler sağlama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Azure Active Directory ile uygulamalar için grup Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Uygulamanız üzerinde Sorunsuz Çoklu Oturum Açma kullanıyorsanız bkz. Kurumsal uygulamalar için [SAML belirtecsinde verilen talepler.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims Özniteliği Eşlemesi**

1. PowerShell kullanarak talep eşleme ilkesi yapılandırmak için [bkz. Kiracıdaki](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)belirli bir uygulama için belirteçlerde talepleri özelleştirme (Önizleme) .
2. Dizin şema uzantısı öznitelikleri, kullanıcı nesnelerinde ve gruplar, kiracı ayrıntıları ve hizmet Azure Active Directory diğer dizin nesnelerinde ek veriler depolamak için bir yol sağlar. Yalnızca kullanıcı nesnelerindeki uzantı öznitelikleri, iddiaları uygulamalara ifade etmek için kullanılabilir. [Taleplerde dizin şema uzantısı özniteliklerinin kullanımı,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) belirteç talebinde kullanıcı verilerini uygulamalara göndermek için dizin şema uzantısı özniteliklerini kullanmayı açıklar.

Belirteç iddiaları hakkında daha fazla bilgi için bkz:

- [Erişim belirteçleri ile ilgili talepler](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Bir davanın id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C tarafından verilen Kimlik belirteçleri ve erişim belirteçleri içinde beklediğiniz talepler
- [SAML belirteci talep başvurusu](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
