---
title: Dynamics 365 - yanlış Pano Dynamics 365 birleştirilmiş arabiriminde gösterilir.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749039"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c8db3-102">Yanlış Pano Dynamics 365 birleştirilmiş arabiriminde gösterilir.</span><span class="sxs-lookup"><span data-stu-id="c8db3-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c8db3-103">Neden beklediğiniz olandan farklı bir Pano görebilirsiniz çeşitli nedenleri vardır:</span><span class="sxs-lookup"><span data-stu-id="c8db3-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c8db3-104">Kullanıcı bir kullanıcı varsayılan pano ayarladı.</span><span class="sxs-lookup"><span data-stu-id="c8db3-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c8db3-105">Bir kullanıcıyı tanımlamak genellikle varsayılan pano ayarlanmışsa Pano komut çubuğunda **Varsayılan olarak belirle** düğmesini göstermez.</span><span class="sxs-lookup"><span data-stu-id="c8db3-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c8db3-106">Kullanıcının varsayılan pano içinde geçerli app olmasa bile, kullanıcı varsayılan pano diğer varsayılan panolar geçersiz kılar.</span><span class="sxs-lookup"><span data-stu-id="c8db3-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c8db3-107">Kendi varsayılan Pano için unset aşağıdaki geçici çözümü kullanın.</span><span class="sxs-lookup"><span data-stu-id="c8db3-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c8db3-108">Yeni bir kişisel pano oluşturun.</span><span class="sxs-lookup"><span data-stu-id="c8db3-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c8db3-109">Yeni bir pano, kullanıcı varsayılan olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="c8db3-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c8db3-110">Bu panoyu silme.</span><span class="sxs-lookup"><span data-stu-id="c8db3-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c8db3-111">Pano Site Haritası ayarlanır</span><span class="sxs-lookup"><span data-stu-id="c8db3-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c8db3-112">Bir Pano seçerek ve 'Varsayılan olarak belirle' altında 'Sistem Özelleştirme' seçme, bir kuruluşun varsayılan pano ayarlamış olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c8db3-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c8db3-113">Ancak, kullanıcı erişimi varsa, site haritası Tasarımcısı'nda tanımlanan Pano bu pano üzerinde öncelik kazanır.</span><span class="sxs-lookup"><span data-stu-id="c8db3-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c8db3-114">Kullanıcıların kuruluş varsayılan olarak ayarladığınız Pano görmek için aşağıdakileri yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="c8db3-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c8db3-115">Bu Pano Site Haritası içinde ayarlama</span><span class="sxs-lookup"><span data-stu-id="c8db3-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c8db3-116">Sitemap tanımlı Pano kullanıcılar için erişimi kaldırmak</span><span class="sxs-lookup"><span data-stu-id="c8db3-116">Remove access to the sitemap defined dashboard for those users</span></span>
