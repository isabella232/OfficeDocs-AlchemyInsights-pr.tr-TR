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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="7d145-102">Belirteç İddiaları ve Öznitelikleriyle ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="7d145-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="7d145-103">**Belirteç iddialarını güncelleştirme, yapılandırma veya kaldırma**</span><span class="sxs-lookup"><span data-stu-id="7d145-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="7d145-104">Azure Active Directory'i (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) kullanarak, bir uygulamayı yetkilendirdikten sonra size verilen yanıt belirtecinde rol talebi için talep türünü özelleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7d145-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="7d145-105">Uygulama geliştiriciler, uygulamalarına gönderilen belirteçlerde hangi talepte yer almak istemedilerini belirtmek için Azure AD uygulamalarında isteğe bağlı talepler kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="7d145-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="7d145-106">Daha fazla bilgi için bkz. [Uygulamanıza isteğe bağlı talepler sağlama.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="7d145-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="7d145-107">[Azure Active Directory ile uygulamalar için grup taleplerini yapılandırma.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="7d145-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="7d145-108">Uygulamanıza Sorunsuz Çoklu Oturum Açma kullanıyorsanız, kurumsal uygulamalar için SAML belirtecinde verilen [taleplere bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="7d145-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="7d145-109">**Claims Özniteliği Eşlemesi**</span><span class="sxs-lookup"><span data-stu-id="7d145-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="7d145-110">PowerShell kullanarak talep eşleme ilkesi yapılandırmak için, kiracıdaki belirli bir uygulama için belirteçlerde karartılan talepler [özelleştirme (Önizleme) bakın.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="7d145-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="7d145-111">Dizin şema uzantısı öznitelikleri, kullanıcı nesnelerinde ve gruplar, kiracı ayrıntıları, hizmet sorumluları gibi diğer dizin nesnelerinde Azure Active Directory'de ek veri depolamak için bir yol sağlar.</span><span class="sxs-lookup"><span data-stu-id="7d145-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="7d145-112">Uygulamaları talep etmek için yalnızca kullanıcı nesnelerindeki uzantı öznitelikleri kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="7d145-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="7d145-113">[Taleplerde dizin şema uzantısı özniteliklerini kullanmak,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) belirteç talebinde kullanıcı verilerini uygulamalara göndermek için dizin şema uzantısı özniteliklerini kullanmayı açıklar.</span><span class="sxs-lookup"><span data-stu-id="7d145-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="7d145-114">Belirteç talebi hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="7d145-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="7d145-115">Erişim belirteçleri için talepler</span><span class="sxs-lookup"><span data-stu-id="7d145-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="7d145-116">Bir iş id_token</span><span class="sxs-lookup"><span data-stu-id="7d145-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="7d145-117">[](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C tarafından verilen kimlik belirteçleri ve erişim belirteçleri ile karşınıza çıkarabilirsiniz iddialar</span><span class="sxs-lookup"><span data-stu-id="7d145-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="7d145-118">SAML belirteci talep başvurusu</span><span class="sxs-lookup"><span data-stu-id="7d145-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
