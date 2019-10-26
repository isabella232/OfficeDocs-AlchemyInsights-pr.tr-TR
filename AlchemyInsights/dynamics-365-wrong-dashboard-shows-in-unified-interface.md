---
title: Dynamics 365 - Dynamics 365 Birleşik Arabiriminde Yanlış Pano Gösterir
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528571"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="29b77-102">Dynamics 365 birleşik arabiriminde yanlış pano gösterir</span><span class="sxs-lookup"><span data-stu-id="29b77-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="29b77-103">Beklediğiniz panodan farklı bir pano görmenizin birkaç nedeni vardır:</span><span class="sxs-lookup"><span data-stu-id="29b77-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="29b77-104">Kullanıcı varsayılan pano belirledi</span><span class="sxs-lookup"><span data-stu-id="29b77-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="29b77-105">Genellikle varsayılan **olarak ayarlı** bir kullanıcı varsayılan panosu nu tanımlayabilirsiniz, pano komut çubuğunda varsayılan olarak ayarlanmaz.</span><span class="sxs-lookup"><span data-stu-id="29b77-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="29b77-106">Kullanıcı varsayılan panosu, kullanıcının varsayılan panosu geçerli uygulamada olmasa bile diğer tüm varsayılan panoları geçersiz kılar.</span><span class="sxs-lookup"><span data-stu-id="29b77-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="29b77-107">Varsayılan panolarını ayarlamak için aşağıdaki geçici çözüme göre kullanın.</span><span class="sxs-lookup"><span data-stu-id="29b77-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="29b77-108">Yeni bir kişisel pano oluşturun.</span><span class="sxs-lookup"><span data-stu-id="29b77-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="29b77-109">Yeni panoyu kullanıcı varsayılanı olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="29b77-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="29b77-110">Şu panoyonu sil.</span><span class="sxs-lookup"><span data-stu-id="29b77-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="29b77-111">Pano site haritasında ayarlanır</span><span class="sxs-lookup"><span data-stu-id="29b77-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="29b77-112">Bir pano seçip 'Sistemi Özelleştir' altında 'Varsayılan Olarak Ayarla' seçeneğini seçerek bir kuruluş varsayılan panosu ayarlamış olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="29b77-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="29b77-113">Ancak, site haritası tasarımcısında tanımlanan pano, kullanıcının bu panoya erişimi varsa, bu panodan önce gelir.</span><span class="sxs-lookup"><span data-stu-id="29b77-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="29b77-114">Kullanıcıların ayarladığınız panoyu kuruluş varsayılanı olarak görmesini sağlamak için şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="29b77-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="29b77-115">Site haritasındaki panoyu ayarlama</span><span class="sxs-lookup"><span data-stu-id="29b77-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="29b77-116">Bu kullanıcılar için site haritası tanımlı panoya erişimi kaldırma</span><span class="sxs-lookup"><span data-stu-id="29b77-116">Remove access to the sitemap defined dashboard for those users</span></span>
