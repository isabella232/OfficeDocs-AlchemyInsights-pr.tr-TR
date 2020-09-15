---
title: Dynamics 365-Dynamics 365 Birleşik arabiriminde yanlış Pano gösteriliyor
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711295"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="2679c-102">Dynamics 365 Birleşik arabiriminde yanlış Pano gösteriliyor</span><span class="sxs-lookup"><span data-stu-id="2679c-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="2679c-103">Beklediğinizden farklı bir panoyu görmenizin birkaç nedeni vardır:</span><span class="sxs-lookup"><span data-stu-id="2679c-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="2679c-104">Kullanıcı varsayılan kullanıcı panosunu ayarladı</span><span class="sxs-lookup"><span data-stu-id="2679c-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="2679c-105">Genellikle, **Varsayılan olarak ayarla** düğmesi Pano komut çubuğunda görünmüyorsa, Kullanıcı varsayılan panosunun ayarlandığını belirleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2679c-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="2679c-106">Kullanıcının varsayılan panosu geçerli uygulamada olmasa bile, Kullanıcı varsayılan panosu tüm diğer varsayılan panoları geçersiz kılar.</span><span class="sxs-lookup"><span data-stu-id="2679c-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="2679c-107">Varsayılan panosunu atamak için aşağıdaki geçici çözümü kullanın.</span><span class="sxs-lookup"><span data-stu-id="2679c-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="2679c-108">Yeni bir kişisel pano oluşturun.</span><span class="sxs-lookup"><span data-stu-id="2679c-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="2679c-109">Yeni panoyu Kullanıcı varsayılanı olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="2679c-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="2679c-110">Panoyu silin.</span><span class="sxs-lookup"><span data-stu-id="2679c-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="2679c-111">Pano Site Haritası 'nda ayarlanır</span><span class="sxs-lookup"><span data-stu-id="2679c-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="2679c-112">Bir panoyu seçip ' Sistemi Özelleştir ' altında ' varsayılan olarak ayarla ' seçeneğini belirleyerek bir kuruluşun varsayılan panosunu ayarlamış olabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2679c-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="2679c-113">Ancak site haritası tasarımcısında tanımlanan Pano bu panoyu, kullanıcının erişimi varsa bu panoda önceliklidir.</span><span class="sxs-lookup"><span data-stu-id="2679c-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="2679c-114">Kullanıcıların kuruluş varsayılanı olarak ayarlamış olduğunuz panoyu görmesi için şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="2679c-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="2679c-115">Bu panoyu site haritası 'nda ayarlama</span><span class="sxs-lookup"><span data-stu-id="2679c-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="2679c-116">Bu kullanıcılar için site haritası tanımlı panoya erişimi kaldırma</span><span class="sxs-lookup"><span data-stu-id="2679c-116">Remove access to the sitemap defined dashboard for those users</span></span>
