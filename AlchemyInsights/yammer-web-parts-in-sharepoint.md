---
title: SharePoint içinde Yammer web parçaları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198385"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="b4cb5-102">SharePoint içinde Yammer web parçaları</span><span class="sxs-lookup"><span data-stu-id="b4cb5-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="b4cb5-103">Yammer Konuşmaları ve Yammer Highlights web bölümleri modern ve klasik SharePoint sayfalarında işbirliğini geliştirir.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="b4cb5-104">Daha fazla bilgi için [Yammer Konuşmaları](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) ve [Yammer Önemli Noktaları'na](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)bakın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="b4cb5-105">Modern Yammer Konuşmaları web bölümü yeni Yammer deneyimi ne kadar güncellenmektedir ve Hedefli Sürüm kiracılar için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="b4cb5-106">GA lansmanı başladı.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-106">GA rollout has started.</span></span> <span data-ttu-id="b4cb5-107">Yeni özellikler arasında herhangi bir gönderiyle (Sorular, Anketler, Övgü) bir konuşma başlatma ve en iyi yanıtları doğrudan SharePoint'ten işaretleme olanağı yer alır.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="b4cb5-108">Daha fazla bilgi için [Yeni Yammer müşteri koşulları ve SSS](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="b4cb5-109">Hangi web bölümünün ve yapılandırmanın sizin için uygun olduğunu anlamak için [bkz.](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)</span><span class="sxs-lookup"><span data-stu-id="b4cb5-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="b4cb5-110">**SharePoint Server ile web bölümlerini kullanma**</span><span class="sxs-lookup"><span data-stu-id="b4cb5-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="b4cb5-111">Web bölümleri, şirket içi ortamlarda ki modern ve klasik sayfalarda kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="b4cb5-112">Modern sayfalar hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019)</span><span class="sxs-lookup"><span data-stu-id="b4cb5-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="b4cb5-113">Klasik sayfalar hakkında daha fazla bilgi için bkz: [SharePoint Servers 2013, 2016 ve 2019'daki klasik bir sayfaya Yammer akışı ekleyin.](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)</span><span class="sxs-lookup"><span data-stu-id="b4cb5-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="b4cb5-114">**Yammer Gömme**</span><span class="sxs-lookup"><span data-stu-id="b4cb5-114">**Yammer Embed**</span></span>  

<span data-ttu-id="b4cb5-115">Embed kullanımını test etmek için Embed Yapılandırması aracını kullanın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="b4cb5-116">Embed için gelecekteki bir güncelleştirme yeni Yammer deneyimini sağlayacaktır.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="b4cb5-117">Daha fazla bilgi için [Yammer Embed Yapılandırma aracına](https://aka.ms/YammerEmbedConfigureTool)bakın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="b4cb5-118">Yammer Embed bileşenini daha iyi anlamak için [Embed Feed'e](https://aka.ms/YammerDevDocs)bakın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="b4cb5-119">**Bilinen sorunlar ve sınırlamalar**</span><span class="sxs-lookup"><span data-stu-id="b4cb5-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="b4cb5-120">Grup iD'leri değiştirilen yeni Yammer URL'lerinden kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="b4cb5-121">URL'lerden grup d'leri veya diğer t'ler almak için klasik moda geri geçin.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="b4cb5-122">Özel (kibir) etki alanları desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="b4cb5-123">Yammer Embed mobil cihazlar için optimize edilmedi.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="b4cb5-124">En iyi deneyimi yaşamak için Yammer Konuşmaları web bölümüne sahip modern sayfaları kullanın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="b4cb5-125">Özel temalar, Yammer Konuşmaları web bölümünün görünümünü ve kullanılabilirliğini etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="b4cb5-126">Sorunları bildirmek için bir destek örneği açın.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-126">Open a support case to report issues.</span></span>