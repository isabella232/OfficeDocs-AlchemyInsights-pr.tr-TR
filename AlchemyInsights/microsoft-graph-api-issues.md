---
title: Microsoft Graph API sorunları
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714517"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="ec1a2-102">Microsoft Graph API sorunları</span><span class="sxs-lookup"><span data-stu-id="ec1a2-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="ec1a2-103">Bu konu, hala Azure AD Graph API kullanan geliştiriciler için de geçerli olabilir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="ec1a2-104">Bununla birlikte, **tüm dizin,** kimlik ve erişim yönetimi senaryolarınız için Microsoft Graph'i kullanmanız kesinlikle önerilir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="ec1a2-105">**Kimlik doğrulama veya yetkilendirme sorunları**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="ec1a2-106">Uygulamanız Microsoft Graph **çağrısı** yapmak için belirteç alamasa da, bu konuda daha özel yardım ve destek almak için erişim belirteci **(Kimlik Doğrulama)** Microsoft Graph kategorisi alma ile ilgili Sorun'u seçin.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="ec1a2-107">Uygulamanız Microsoft Graph'i arama sırasında **401 veya 403** yetkilendirme hatası alıyorsa, bu konuda daha özel yardım ve destek almak için Erişim reddedildi hatası **(Yetkilendirme)** Microsoft Graph API kategorisini seçin.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="ec1a2-108">**Microsoft Graph'i kullanmak istiyorum, ancak nereden başlayacağımdan emin değilim**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="ec1a2-109">Microsoft Graph'a genel bakış</span><span class="sxs-lookup"><span data-stu-id="ec1a2-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="ec1a2-110">Microsoft Graph'te Kimlik ve Erişim Yönetimine Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="ec1a2-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="ec1a2-111">Microsoft Graph uygulamaları yapmaya başlama</span><span class="sxs-lookup"><span data-stu-id="ec1a2-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="ec1a2-112">**Microsoft Graph Explorer** - Kiracı veya tanıtım kiracısı içinde Microsoft Graph API'lerini test</span><span class="sxs-lookup"><span data-stu-id="ec1a2-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="ec1a2-113">**Microsoft Graph'i kullanmak istiyorum, ancak ihtiyacım olan v1.0 dizin API'lerini destekliyor mu?**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="ec1a2-114">Microsoft Graph dizin, kimlik ve erişim yönetimi için önerilen API'dir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="ec1a2-115">Bununla birlikte, Azure AD Graph ve Microsoft Graph'te mümkün olan şeyler arasında hala birkaç boşluk vardır.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="ec1a2-116">Seçiminize yardımcı olmak için en güncel farkları vurgulayan aşağıdaki makaleleri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="ec1a2-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="ec1a2-117">Azure AD Graph ile Microsoft Graph arasındaki kaynak türü farklılıkları</span><span class="sxs-lookup"><span data-stu-id="ec1a2-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="ec1a2-118">Azure AD Graph ile Microsoft Graph arasındaki özellik farklılıkları</span><span class="sxs-lookup"><span data-stu-id="ec1a2-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="ec1a2-119">Azure AD ile Microsoft Graph arasındaki yöntem farklılıkları</span><span class="sxs-lookup"><span data-stu-id="ec1a2-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="ec1a2-120">**Çağrı yapacağım API çalışmıyor, daha fazla test nereden yapabilirim?**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="ec1a2-121">**Microsoft Graph Explorer** - Kiracınız veya tanıtım kiracısı olan Microsoft Graph API'lerini test edin ve Microsoft Graph Explorer'daki **örnek** sorgulara göz atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="ec1a2-122">**Uygulamam çok yavaş ve aynı zamanda kısıtlanıyor. Hangi geliştirmeleri ben yapmak için?**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="ec1a2-123">Senaryona bağlı olarak, uygulamanızı daha iyi performans ortaya çıkarmanızı ve bazı durumlarda da hizmet tarafından azaltmaya (çok fazla arama yaparken) daha az açık hale gelen çeşitli seçenekler vardır.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="ec1a2-124">Microsoft Graph en iyi yöntemleri</span><span class="sxs-lookup"><span data-stu-id="ec1a2-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="ec1a2-125">Toplu istekler</span><span class="sxs-lookup"><span data-stu-id="ec1a2-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="ec1a2-126">Değişiklik sorgusu aracılığıyla değişiklikleri izleme</span><span class="sxs-lookup"><span data-stu-id="ec1a2-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="ec1a2-127">Web'ler aracılığıyla değişikliklerle ilgili bilgi al</span><span class="sxs-lookup"><span data-stu-id="ec1a2-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="ec1a2-128">Azaltma kılavuzu</span><span class="sxs-lookup"><span data-stu-id="ec1a2-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="ec1a2-129">**Hatalar ve bilinen sorunlar hakkında nereden daha fazla bilgi bulamıyorum?**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="ec1a2-130">Microsoft Graph hata yanıt bilgileri</span><span class="sxs-lookup"><span data-stu-id="ec1a2-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="ec1a2-131">Microsoft Graph ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="ec1a2-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="ec1a2-132">**Hizmet kullanılabilirliği ve bağlantısının durumunu nereden kontrol edeceğim?**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="ec1a2-133">Microsoft Graph aracılığıyla erişilebilen temel hizmetlerin hizmet kullanılabilirliği ve bağlantısı, Microsoft Graph'in genel kullanılabilirliğini ve performansını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="ec1a2-134">Azure Active Directory hizmetinin durumu için, Azure durum sayfasında listelenen **Güvenlik + Kimlik** hizmetlerinin durumunu kontrol [edin.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="ec1a2-135">Microsoft Graph'e katkıda bulunan Office hizmetleri için, Office Hizmet Durumu Panosunda listelenen [hizmetlerin durumunu kontrol edin.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ec1a2-136">Microsoft Graph yetkilendirme hataları, çoğu 401 veya 403 hatası oluşturan çeşitli sorunların sonucu olabilir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="ec1a2-137">Örneğin, aşağıdakilerin hepsi yetkilendirme hatalarına neden olabilir:</span><span class="sxs-lookup"><span data-stu-id="ec1a2-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="ec1a2-138">Yanlış [erişim belirteci edinme akışları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="ec1a2-139">Kötü yapılandırılmış [izin kapsamları](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="ec1a2-140">[Onay](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) eksikliği</span><span class="sxs-lookup"><span data-stu-id="ec1a2-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="ec1a2-141">\**_Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) desteğinin sonu_* _</span><span class="sxs-lookup"><span data-stu-id="ec1a2-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="ec1a2-142">_*30 Haziran 2020'den itibaren*\* artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ec1a2-143">Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="ec1a2-144">**30 Haziran 2022'den** başlayarak, ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="ec1a2-145">Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*</span><span class="sxs-lookup"><span data-stu-id="ec1a2-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="ec1a2-146">Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktasının yanıtlarını almayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ec1a2-147">**ADAL Geçişi**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-147">**ADAL Migration**</span></span>

<span data-ttu-id="ec1a2-148">En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="ec1a2-149">Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="ec1a2-150">ADAL SSS bölümünü okuyunuz</span><span class="sxs-lookup"><span data-stu-id="ec1a2-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="ec1a2-151">Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="ec1a2-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="ec1a2-152">Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISV'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ec1a2-153">Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="ec1a2-154">**AAD Graph Geçişi**</span><span class="sxs-lookup"><span data-stu-id="ec1a2-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="ec1a2-155">Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını Microsoft Graph'e geçirme [yönergelerimizi izleyin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="ec1a2-156">[Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="ec1a2-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="ec1a2-157">Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="ec1a2-158">Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ec1a2-159">Microsoft desteği, kiracınız için tüm AAD Graph kullanımının bir listesini de sağlar.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="ec1a2-160">Uygulamanın Microsoft Graph'te verilere erişmesi için, kullanıcı veya yöneticinin izin süreci aracılığıyla ona doğru izinleri ataması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="ec1a2-161">[Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) her bir önemli Microsoft Graph API'leri kümesiyle ilişkilendirilmiş izinleri listeler.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="ec1a2-162">Ayrıca, izinleri kullanma konusunda da yol göstermeyi sağlar.</span><span class="sxs-lookup"><span data-stu-id="ec1a2-162">It also provides guidance about how to use the permissions.</span></span>
