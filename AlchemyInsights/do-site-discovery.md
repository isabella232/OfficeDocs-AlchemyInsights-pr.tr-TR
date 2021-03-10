---
title: Site bulma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694554"
---
# <a name="do-site-discovery"></a><span data-ttu-id="68eea-102">Site bulma</span><span class="sxs-lookup"><span data-stu-id="68eea-102">Do site discovery</span></span>

<span data-ttu-id="68eea-103">Organizasyonunız hala eski web uygulamalarını ve Internet Explorer modunu kullanmayı planlıyorsa (çoğu müşteri bunu kullanıyorsa), bazı ek site keşifleri yapsanız iyi olur.</span><span class="sxs-lookup"><span data-stu-id="68eea-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="68eea-104">**Microsoft Edge'in eski bir sürümünü zaten dağıttın**</span><span class="sxs-lookup"><span data-stu-id="68eea-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="68eea-105">Kurumsal Site Listenizi Microsoft Edge'in eski sürümüyle çalışacak şekilde zaten yapılandırdıysanız, site bulmanız neredeyse bitti.</span><span class="sxs-lookup"><span data-stu-id="68eea-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="68eea-106">Tek ihtiyacınız olan nötr siteler eklemektir.</span><span class="sxs-lookup"><span data-stu-id="68eea-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="68eea-107">Nötr siteler genellikle çoklu oturum açma (SSO) sağlayan sitelerdir.</span><span class="sxs-lookup"><span data-stu-id="68eea-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="68eea-108">Microsoft Edge'den nötr bir siteye gidersiniz, kimlik doğrulaması yapmak için Microsoft Edge'de kalmak istersiniz.</span><span class="sxs-lookup"><span data-stu-id="68eea-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="68eea-109">Internet Explorer modunda nötr bir siteye gidersiniz, kimlik doğrulaması yapmak için Internet Explorer modunda kalmak istersiniz.</span><span class="sxs-lookup"><span data-stu-id="68eea-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="68eea-110">Herhangi bir SSO veya diğer nötr siteleri kullanın ve bunları Kurumsal Site Listenize ekleyin.</span><span class="sxs-lookup"><span data-stu-id="68eea-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="68eea-111">**Internet Explorer varsayılan tarayıcınızdır**</span><span class="sxs-lookup"><span data-stu-id="68eea-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="68eea-112">Şu anda yalnızca Internet Explorer kullanıyorsanız, hangi sitelerin modern web standartlarına yükseltil olduğunu ve hangilerinin hala Internet Explorer'ın gerekli olduğunu bilmiyor olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="68eea-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="68eea-113">Internet Explorer modunu yalnızca bu siteler için kullanasınız diye bu siteleri bulmak ve Kurumsal Site Listesi'ne eklemek istiyor olursunuz.</span><span class="sxs-lookup"><span data-stu-id="68eea-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="68eea-114">[Kurumsal Site Bulma,](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) Internet Explorer modu gerektiren siteler keşfeder.</span><span class="sxs-lookup"><span data-stu-id="68eea-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="68eea-115">Windows 10, Windows 8.1 veya Windows 7'de Windows Internet Explorer 8 ile Internet Explorer 11 arasında çalışan bilgisayarlarda veri toplayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="68eea-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="68eea-116">**Verileri çözümleme**</span><span class="sxs-lookup"><span data-stu-id="68eea-116">**Analyze the data**</span></span>

<span data-ttu-id="68eea-117">Site verilerini topladikten sonra, verileri çözümlemek için aşağıdaki dört adımlık süreci öneririz:</span><span class="sxs-lookup"><span data-stu-id="68eea-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="68eea-118">Verileri etki alanına ve ardından URL'ye göre sırala.</span><span class="sxs-lookup"><span data-stu-id="68eea-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="68eea-119">Internet Explorer modu için yapılandırılan bir uygulamanın sınırlarını tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="68eea-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="68eea-120">Uygulamayı tanımlayan tüm siteleri ve web denetimlerini eklemek istiyor, ancak fazladan siteler ve denetimler eklemek istemiyorsanız.</span><span class="sxs-lookup"><span data-stu-id="68eea-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="68eea-121">Bazı siteler aynı şekilde basit *https://contoso.com/app1* olabilir, ancak diğerleri birden çok site ve sayfa tanımlamanız gerektirmektedir.</span><span class="sxs-lookup"><span data-stu-id="68eea-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="68eea-122">Yerel olarak çalışmay olmadığını doğrulamak için uygulamayı test edin.</span><span class="sxs-lookup"><span data-stu-id="68eea-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="68eea-123">Birçok site modern bir tarayıcı algılayana kadar modern içerik sağlar ve yalnızca Internet Explorer'ı algılayana kadar eski içerik sağlar.</span><span class="sxs-lookup"><span data-stu-id="68eea-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="68eea-124">Uygulamayı test başarısız olursa Kurumsal Site Listeniz'e ekleyin.</span><span class="sxs-lookup"><span data-stu-id="68eea-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="68eea-125">En iyi uygulama olarak, uygulamayı oluşturan tüm siteleri grupla.</span><span class="sxs-lookup"><span data-stu-id="68eea-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="68eea-126">Bu şekilde, bir uygulamayı yükseltken sitenin tamamını Internet Explorer modundan kaldırmak ve bu uygulama için modern bir tarayıcı kullanmaya başlamak daha kolaydır.</span><span class="sxs-lookup"><span data-stu-id="68eea-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="68eea-127">Site bulma işi bittiğinde ve verileri analiz ettiyken, kanal stratejinize bakmaya başlamaya hazır oluruz.</span><span class="sxs-lookup"><span data-stu-id="68eea-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

