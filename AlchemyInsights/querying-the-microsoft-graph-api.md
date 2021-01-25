---
title: Microsoft Graph API 'YI sorgulama
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974689"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="9fe76-102">Microsoft Graph API 'YI sorgulama</span><span class="sxs-lookup"><span data-stu-id="9fe76-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="9fe76-103">Bu konu, hala Azure AD grafik API 'sini kullanan geliştiriciler için de geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="9fe76-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="9fe76-104">Ancak, tüm dizin, kimlik ve erişim yönetimi senaryolarınız için Microsoft Graph kullanmanız **kesinlikle** önerilir.</span><span class="sxs-lookup"><span data-stu-id="9fe76-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="9fe76-105">**Kimlik doğrulama veya yetkilendirme sorunları**</span><span class="sxs-lookup"><span data-stu-id="9fe76-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="9fe76-106">Uygulamanız Microsoft Graph 'ı aramak için **belirteçleri edinemiyorsanız** , bu konuda daha belirli yardım ve destek almak için **erişim belirteci (kimlik doğrulama) alma hakkında sorun** seçin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="9fe76-107">Uygulamanız Microsoft Graph 'ı ararken **401 veya 403 yetkilendirme hataları** alıyorsa, bu konuda daha ayrıntılı yardım almak için **erişim reddedildi hatasını alma (yetkilendirme)** Microsoft Graph API kategorisini seçin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="9fe76-108">**Microsoft Graph 'ı kullanmak istiyorum, ancak nereden başlayacağınızdan emin değil**</span><span class="sxs-lookup"><span data-stu-id="9fe76-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="9fe76-109">Microsoft Graph hakkında daha fazla bilgi edinmek için bkz:</span><span class="sxs-lookup"><span data-stu-id="9fe76-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="9fe76-110">Microsoft Graph 'a genel bakış</span><span class="sxs-lookup"><span data-stu-id="9fe76-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="9fe76-111">Microsoft Graph 'ta kimlik ve erişim yönetimine genel bakış</span><span class="sxs-lookup"><span data-stu-id="9fe76-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="9fe76-112">Microsoft Graph uygulamalarını oluşturmaya başlarken</span><span class="sxs-lookup"><span data-stu-id="9fe76-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="9fe76-113">**Microsoft Graph Explorer** -kiracınızdaki veya bir tanıtım kiracısındaki Microsoft Graph API 'lerini test edin</span><span class="sxs-lookup"><span data-stu-id="9fe76-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="9fe76-114">**Microsoft Graph 'ı kullanmak istiyorum, ancak ihtiyacım olan v 1.0 Dizin API 'Lerini destekliyor mu?**</span><span class="sxs-lookup"><span data-stu-id="9fe76-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="9fe76-115">Microsoft Graph, dizin, kimlik ve erişim yönetimi için önerilen API 'dır.</span><span class="sxs-lookup"><span data-stu-id="9fe76-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="9fe76-116">Ancak, Azure AD Graph ve Microsoft Graph 'ta mümkün olduğunca birkaç boşluk vardır.</span><span class="sxs-lookup"><span data-stu-id="9fe76-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="9fe76-117">Seçiminize yardımcı olmak için en güncel farklılıkları vurgulayan aşağıdaki makaleleri gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="9fe76-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="9fe76-118">Azure AD grafiği ile Microsoft Graph arasındaki kaynak türü farklılıkları</span><span class="sxs-lookup"><span data-stu-id="9fe76-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="9fe76-119">Azure AD Graph ve Microsoft Graph arasındaki özellik farklılıkları</span><span class="sxs-lookup"><span data-stu-id="9fe76-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="9fe76-120">Azure AD ve Microsoft Graph arasındaki yöntem farklılıkları</span><span class="sxs-lookup"><span data-stu-id="9fe76-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="9fe76-121">***Kullanıcı* nesnesini sorgulıyorum, özelliklerinin çoğu eksik**</span><span class="sxs-lookup"><span data-stu-id="9fe76-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="9fe76-122">`GET https://graph.microsoft.com/v1.0/users` Microsoft Graph, döndürülecek varsayılan *Kullanıcı* özellikleri kümesini otomatik olarak seçtiği için, yalnızca 11 özellik verir.</span><span class="sxs-lookup"><span data-stu-id="9fe76-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="9fe76-123">Başka *Kullanıcı* özelliklerine ihtiyaç duyarsanız, uygulamanızın ihtiyaç duyduğu özellikleri seçmek için $Select kullanın.</span><span class="sxs-lookup"><span data-stu-id="9fe76-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="9fe76-124">Önce **Microsoft Graph Explorer** 'da deneyin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="9fe76-125">**Bazı Kullanıcı özelliği değerleri, ayarladığım bilinmekle aynı şekilde *null***</span><span class="sxs-lookup"><span data-stu-id="9fe76-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="9fe76-126">En büyük olasılık açıklaması, uygulamaya kullanıcının verilmesinden kaynaklanır *. Readbasıc. All* izni.</span><span class="sxs-lookup"><span data-stu-id="9fe76-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="9fe76-127">Bu, uygulamanın daha önce ayarlamış olsalar bile tüm diğer özellikleri null olarak döndürmesinin, sınırlı Kullanıcı özellikleri kümesini okumasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="9fe76-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="9fe76-128">Uygulama *kullanıcısına* izin vermeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="9fe76-129">Daha fazla bilgi için [Microsoft Graph Kullanıcı izinleri](https://docs.microsoft.com/graph/permissions-reference#user-permissions)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="9fe76-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="9fe76-130">**İsteklerim 'deki verileri filtrelemek için OData sorgu parametrelerini kullanırken sorun yaşıyorum**</span><span class="sxs-lookup"><span data-stu-id="9fe76-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="9fe76-131">Microsoft Graph, çok sayıda OData sorgu parametresini destekleirken, bu parametrelerin çoğu Microsoft Graph 'ta Dizin Hizmetleri ( *Directoryobject*'den devralan kaynaklar) tarafından tam olarak desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="9fe76-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="9fe76-132">Microsoft Graph 'ta, Azure AD grafiğinde bulunan sınırlamalar da korunur:</span><span class="sxs-lookup"><span data-stu-id="9fe76-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="9fe76-133">**Desteklenmiyor**: *null* veya *olmayan* null değerleri $Count, $Search ve $Filter</span><span class="sxs-lookup"><span data-stu-id="9fe76-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="9fe76-134">**Desteklenmiyor**: belirli özelliklerde $Filter (hangi özelliklere filtre uygulanamayacak kaynak konularına bakın)</span><span class="sxs-lookup"><span data-stu-id="9fe76-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="9fe76-135">**Desteklenmiyor**: sayfalandırma, filtreleme ve aynı anda sıralama</span><span class="sxs-lookup"><span data-stu-id="9fe76-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="9fe76-136">**Desteklenmiyor**: ilişkide filtreleme.</span><span class="sxs-lookup"><span data-stu-id="9fe76-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="9fe76-137">Örneğin, İngiltere grubunun İngiltere 'deki tüm üyelerini bulun.</span><span class="sxs-lookup"><span data-stu-id="9fe76-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="9fe76-138">**Kısmi destek**: *kullanıcıya* $OrderBy (yalnızca DisplayName ve UserPrincipalName) ve *Grup*</span><span class="sxs-lookup"><span data-stu-id="9fe76-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="9fe76-139">**Kısmi destek**: $Filter (tek bir nesnenin ilişkilerini yalnızca *EQ* *,* *StartsWith*, *and ve* Limited *)* desteği, $Expand (tek nesnenin ilişkilerini genişletme tüm ilişkileri döndürür, ancak nesnelerin ilişkilerinin bir koleksiyonunu genişletme sınırlıdır)</span><span class="sxs-lookup"><span data-stu-id="9fe76-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="9fe76-140">Daha fazla bilgi [için bkz.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="9fe76-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="9fe76-141">**Aradığım API çalışmıyor-daha fazla testi nasıl yapabilirim?**</span><span class="sxs-lookup"><span data-stu-id="9fe76-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="9fe76-142">**Microsoft Graph Explorer** -kiracınızdaki veya bir gösteri kiracısındaki Microsoft Graph API 'lerini test edin ve Microsoft Graph Explorer 'daki **örnek sorguları** inceleyin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="9fe76-143">**Verileri sorgulıyorum ancak tamamlanmamış bir veri kümesi aldığımda**</span><span class="sxs-lookup"><span data-stu-id="9fe76-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="9fe76-144">Bir koleksiyonu sorgulamakta ( *Kullanıcılar* gibi), Microsoft Graph sunucu tarafı sayfa sınırlarını kullanır, böylece sonuçlar her zaman varsayılan sayfa boyutuyla döndürülür.</span><span class="sxs-lookup"><span data-stu-id="9fe76-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="9fe76-145">Uygulamanız her zaman hizmetten gelen koleksiyonlar aracılığıyla Page 'i beklemelidir.</span><span class="sxs-lookup"><span data-stu-id="9fe76-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="9fe76-146">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="9fe76-146">For more information, see:</span></span>

- [<span data-ttu-id="9fe76-147">Microsoft Graph en iyi uygulamalar</span><span class="sxs-lookup"><span data-stu-id="9fe76-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="9fe76-148">Uygulamanızda Microsoft Graph verilerini sayfalama</span><span class="sxs-lookup"><span data-stu-id="9fe76-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="9fe76-149">**Uygulamam çok yavaş ve aynı zamanda daraltıldı. Hangi geliştirmeleri yapabilirim?**</span><span class="sxs-lookup"><span data-stu-id="9fe76-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="9fe76-150">Senaryonuza bağlı olarak, uygulamanızı daha iyi hale getirmek için ve bazı durumlarda hizmet tarafından daraltıldı (çok fazla arama yaparken) daha ucuz bir dizi farklı seçenek vardır.</span><span class="sxs-lookup"><span data-stu-id="9fe76-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="9fe76-151">Daha fazla bilgi için şu makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="9fe76-151">To learn more, see:</span></span>

- [<span data-ttu-id="9fe76-152">Microsoft Graph en iyi uygulamalar</span><span class="sxs-lookup"><span data-stu-id="9fe76-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="9fe76-153">İstekleri toplu işleme</span><span class="sxs-lookup"><span data-stu-id="9fe76-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="9fe76-154">Delta sorgusunda değişiklikleri izleme</span><span class="sxs-lookup"><span data-stu-id="9fe76-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="9fe76-155">Web kancaları aracılığıyla değişiklikleri öğrenin</span><span class="sxs-lookup"><span data-stu-id="9fe76-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="9fe76-156">Azaltma Kılavuzu</span><span class="sxs-lookup"><span data-stu-id="9fe76-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="9fe76-157">**Hatalar ve bilinen sorunlar hakkında daha fazla bilgiyi nerede bulabilirim?**</span><span class="sxs-lookup"><span data-stu-id="9fe76-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="9fe76-158">Microsoft Graph hata yanıtı bilgileri</span><span class="sxs-lookup"><span data-stu-id="9fe76-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="9fe76-159">Microsoft Graph ile ilgili bilinen sorunlar</span><span class="sxs-lookup"><span data-stu-id="9fe76-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="9fe76-160">**Hizmet kullanılabilirliği ve bağlantısının durumunu nereden denetleyebilirim?**</span><span class="sxs-lookup"><span data-stu-id="9fe76-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="9fe76-161">Microsoft Graph aracılığıyla erişilebilecek temel hizmetlerin hizmet kullanılabilirliği ve bağlantısı, Microsoft Graph 'ın genel kullanılabilirliğini ve performansını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="9fe76-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="9fe76-162">Azure Active Directory hizmeti durumu için, [Azure durum sayfasında](https://azure.microsoft.com/status/)listelenen **güvenlik + kimlik** hizmetlerinin durumunu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="9fe76-163">Microsoft Graph 'a katkıda bulunan Office Hizmetleri için, [Office hizmet durumu panosunda](https://portal.office.com/adminportal/home#/servicehealth)listelenen hizmetlerin durumunu denetleyin.</span><span class="sxs-lookup"><span data-stu-id="9fe76-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
