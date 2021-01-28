---
title: Belirteç İddiaları ve Öznitelikleriyle ilgili sorunlar
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036080"
---
# <a name="issues-with-token-claims-and-attributes"></a>Belirteç İddiaları ve Öznitelikleriyle ilgili sorunlar

**Belirteç iddialarını güncelleştirme, yapılandırma veya kaldırma**

1. Azure Active Directory'i (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) kullanarak, bir uygulamayı yetkilendirdikten sonra size verilen yanıt belirtecinde rol talebi için talep türünü özelleştirebilirsiniz.
2. Uygulama geliştiriciler, uygulamalarına gönderilen belirteçlerde hangi talepte yer almak istemedilerini belirtmek için Azure AD uygulamalarında isteğe bağlı talepler kullanabilir. Daha fazla bilgi için bkz. [Uygulamanıza isteğe bağlı talepler sağlama.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Azure Active Directory ile uygulamalar için grup taleplerini yapılandırma.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Uygulamanıza Sorunsuz Çoklu Oturum Açma kullanıyorsanız, kurumsal uygulamalar için SAML belirtecinde verilen [taleplere bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Claims Özniteliği Eşlemesi**

1. PowerShell kullanarak talep eşleme ilkesi yapılandırmak için, kiracıdaki belirli bir uygulama için belirteçlerde karartılan talepler [özelleştirme (Önizleme) bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Dizin şema uzantısı öznitelikleri, kullanıcı nesnelerinde ve gruplar, kiracı ayrıntıları, hizmet sorumluları gibi diğer dizin nesnelerinde Azure Active Directory'de ek veri depolamak için bir yol sağlar. Uygulamaları talep etmek için yalnızca kullanıcı nesnelerindeki uzantı öznitelikleri kullanılabilir. [Taleplerde dizin şema uzantısı özniteliklerini kullanmak,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) belirteç talebinde kullanıcı verilerini uygulamalara göndermek için dizin şema uzantısı özniteliklerini kullanmayı açıklar.

Belirteç talebi hakkında daha fazla bilgi için bkz:

- [Erişim belirteçleri için talepler](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Bir iş id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C tarafından verilen kimlik belirteçleri ve erişim belirteçleri ile karşınıza çıkarabilirsiniz iddialar
- [SAML belirteci talep başvurusu](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
