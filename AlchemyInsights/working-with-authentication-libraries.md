---
title: Kimlik Doğrulama Kitaplıkları ile çalışma
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036865"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="df9c8-102">Kimlik Doğrulama Kitaplıkları ile çalışma</span><span class="sxs-lookup"><span data-stu-id="df9c8-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="df9c8-103">Microsoft Kimlik Doğrulama Kitaplığı (MSAL) sorununu çözmek için, aşağıdaki önerilen adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="df9c8-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="df9c8-104">**MSAL :** [Microsoft kimlik platformu kimlik doğrulama kitaplıkları](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) ile çalışma - Bu makalede, çeşitli uygulama türleri için Microsoft Kimlik Doğrulama Kitaplığı desteği açıklanmıştır.</span><span class="sxs-lookup"><span data-stu-id="df9c8-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="df9c8-105">Kitaplık kaynak kodunun bağlantılarını içerir; uygulama projenizin paketini nereden edinebilirsiniz; ve kitaplığın kullanıcı oturum açmasını (kimlik doğrulama), korumalı web API'lerine erişimi (yetkilendirme) veya her ikisini birden destekleyip desteklemeyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="df9c8-106">**Kimlik Doğrulama Sorunlarını** Giderme: MSAL, farklı uygulama senaryolarında kullanmak üzere çeşitli kimlik doğrulama akışlarını destekler.</span><span class="sxs-lookup"><span data-stu-id="df9c8-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="df9c8-107">İstemci uygulamanın nasıl yerleşik olduğunu bağlı olarak, MSAL Microsoft kimlik platformu tarafından desteklenen kimlik doğrulama akışlarından birini veya daha fazlasını kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="df9c8-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="df9c8-108">Bu akışlar, çeşitli türde belirteç ve yetkilendirme kodları üretebilirsiniz ve bunların çalışması için farklı belirteçler gerekli olabilir.</span><span class="sxs-lookup"><span data-stu-id="df9c8-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="df9c8-109">**Erişim Belirteçleri:** [Microsoft kimlik platformu erişim belirteçleri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API'nizin bir erişim belirteci içindeki talepleri nasıl doğrulaya ve kullanabileceğini öğrenin.</span><span class="sxs-lookup"><span data-stu-id="df9c8-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="df9c8-110">Bu makaledeki tüm belgeler, not edildi dışındaki yalnızca kayıtlı API'ler için verilen belirteçlere uygulanır.</span><span class="sxs-lookup"><span data-stu-id="df9c8-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="df9c8-111">Microsoft'a ait API'ler için verilen belirteçler için geçerli değildir ve bu belirteçler, Microsoft kimlik platformunun sizin oluşturtuz bir API için belirteçleri nasıl çıkartır olacağını doğrulamak için kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="df9c8-112">**Azure Active Directory Kimlik Doğrulama Kitaplığı (ADAL) için destek sonu**</span><span class="sxs-lookup"><span data-stu-id="df9c8-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="df9c8-113">**30 Haziran 2020'den** itibaren artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek.</span><span class="sxs-lookup"><span data-stu-id="df9c8-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="df9c8-114">Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.</span><span class="sxs-lookup"><span data-stu-id="df9c8-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="df9c8-115">**30 Haziran 2022'den başlayarak,** ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.</span><span class="sxs-lookup"><span data-stu-id="df9c8-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="df9c8-116">Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek veya *güvenlik güncelleştirmelerini almayacaktır.*</span><span class="sxs-lookup"><span data-stu-id="df9c8-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="df9c8-117">Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktalarından yanıt alamaz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="df9c8-118">**ADAL Geçişi**</span><span class="sxs-lookup"><span data-stu-id="df9c8-118">**ADAL Migration**</span></span>

- <span data-ttu-id="df9c8-119">En son özelliklere ve güvenlik güncelleştirmelerine sahip olan MSAL'a güncelleştirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="df9c8-120">Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.</span><span class="sxs-lookup"><span data-stu-id="df9c8-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="df9c8-121">[ADAL SSS bölümünü okuyun.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="df9c8-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="df9c8-122">[Uygulamaları platform başına nasıl geçirilir hakkında bilgi edinin.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="df9c8-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="df9c8-123">Uygulama platformunun kılavuzunu okuduktan sonra başka sorularınız varsa, [Microsoft Q&A'da](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) [azure-ad-adal-deprecation] etiketiyle gönderide bulunabilir veya kitaplığın GitHub deposunda bir sorun açabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="df9c8-124">Her [kitaplığın](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) repo bağlantıları için **MSAL genel bakış** makalesinde Diller ve çerçeveler bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="df9c8-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="df9c8-125">**Uygulamalardan hangilerinin ADAL'ı kullanabileceğini** anlamanız için yardıma ihtiyacınız varsa, uygulamalarınızı tüm kaynak kodunu gözden geçirmenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="df9c8-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="df9c8-126">Uygunsa, herhangi bir Bağımsız yazılım satıcılarına (ISV) veya uygulama sağlayıcılarına erişin.</span><span class="sxs-lookup"><span data-stu-id="df9c8-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="df9c8-127">Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="df9c8-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







