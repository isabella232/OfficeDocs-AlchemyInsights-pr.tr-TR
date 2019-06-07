---
title: SharePoint çevrimiçi kısıtlamak için Klasik mod
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761779"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="788d9-102">SharePoint çevrimiçi kısıtlamak için Klasik mod</span><span class="sxs-lookup"><span data-stu-id="788d9-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="788d9-103">Bazı kuruluşlar, yine Klasik mod deneyimi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="788d9-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="788d9-104">Klasik mod parçalı düzeyde kaldırmak için hiçbir planları olsa da, artık bir kuruluş (Kiracı) listeler ve kitaplıklar için Klasik mod sınırlamak mümkündür.</span><span class="sxs-lookup"><span data-stu-id="788d9-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="788d9-105">Admin tek tek listeler ve kitaplıklar Klasik modunda aşağıdaki düzeylerde sağladığımız parçalı çevirme anahtarları kullanarak yönetmek için aşağıdaki seçeneğiniz olacaktır:</span><span class="sxs-lookup"><span data-stu-id="788d9-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="788d9-106">Site koleksiyonu</span><span class="sxs-lookup"><span data-stu-id="788d9-106">site collection</span></span>
- <span data-ttu-id="788d9-107">Site</span><span class="sxs-lookup"><span data-stu-id="788d9-107">site</span></span>
- <span data-ttu-id="788d9-108">Liste</span><span class="sxs-lookup"><span data-stu-id="788d9-108">list</span></span>
- <span data-ttu-id="788d9-109">Kitaplığı</span><span class="sxs-lookup"><span data-stu-id="788d9-109">library</span></span>

<span data-ttu-id="788d9-110">Ayrıca, belirli özellikleri kullanan listeleri ve modern tarafından desteklenmeyen özelleştirmeleri yine otomatik olarak Klasik moda bırakılacak.</span><span class="sxs-lookup"><span data-stu-id="788d9-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="788d9-111">1 Nisan 2019, Kiracı düzeyi devre dışı bırakma işlemi başlayan opt dışında modern liste ve kitaplıkları Başlat ve 31 Mayıs 2019 devam.</span><span class="sxs-lookup"><span data-stu-id="788d9-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="788d9-112">Klasik mod Kiracı çevirme sonucu olan kitaplıkları ve listeleri otomatik olarak modern için kaydırılır.</span><span class="sxs-lookup"><span data-stu-id="788d9-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="788d9-113">Klasik mod gerekiyorsa lütfen daha fazla bilgi bakın [burada](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ve PnP Powershell talimatı seçenekleri ve bugün Klasik mod deneyimi kullanmak için kullanabileceğiniz araçları açıklar [burada](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) .</span><span class="sxs-lookup"><span data-stu-id="788d9-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
