---
title: SAML Onaylamaları (Belirteçler)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109260"
---
# <a name="saml-assertions-tokens"></a>SAML Onaylamaları (Belirteçler)

1. Güvenlik Onaylama Dili (SAML) belirteçleri, taleplerin XML temsilleridir. Varsayılan olarak, Communication Foundation (WCF) Windows federasyon güvenlik senaryolarında kullandığı SAML belirteçleri belirteç olarak ve edilir. Daha fazla bilgi için [bkz. SAML Belirteçleri ve Talep.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Bu Microsoft kimlik platformu, her kimlik doğrulama akışının iş akışında çeşitli türde güvenlik belirteci sağlar. [SAML belirteci](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) talep başvurusu, SAML 2.0 belirteçlerinin biçimini, güvenlik özelliklerini ve içeriğini açıklar.
3. Belirteç yaşam sürelerini [yapılandırmayı anlamak için Microsoft kimlik platformu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) belirteç yaşam ömrü yönergelerini izleyin.
4. Azure AD SAML belirteç [şifrelemesi'nin](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) nasıl yapılandırıldığından emin olmak için bu makalede belirtilen adımları izleyin.
5. Azure AD'de, sertifika imzalama seçeneklerini ve sertifika imzalama algoritmasını kurabilirsiniz. Daha fazla bilgi için bkz. Azure Active Directory'daki galeri uygulamaları için [SAML belirtecinde gelişmiş sertifika Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
