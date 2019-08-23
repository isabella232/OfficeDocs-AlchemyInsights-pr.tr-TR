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
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551579"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="3e65f-102">SharePoint çevrimiçi kısıtlamak için Klasik mod</span><span class="sxs-lookup"><span data-stu-id="3e65f-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="3e65f-103">Bazı kuruluşlar, yine Klasik mod deneyimi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="3e65f-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="3e65f-104">Klasik mod parçalı düzeyde kaldırmak için hiçbir planları olsa da, artık bir kuruluş (Kiracı) listeler ve kitaplıklar için Klasik mod sınırlamak mümkündür.</span><span class="sxs-lookup"><span data-stu-id="3e65f-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="3e65f-105">Admin tek tek listeler ve kitaplıklar Klasik modunda aşağıdaki düzeylerde sağladığımız parçalı çevirme anahtarları kullanarak yönetmek için aşağıdaki seçeneğiniz olacaktır:</span><span class="sxs-lookup"><span data-stu-id="3e65f-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="3e65f-106">Site koleksiyonu</span><span class="sxs-lookup"><span data-stu-id="3e65f-106">site collection</span></span>
- <span data-ttu-id="3e65f-107">Site</span><span class="sxs-lookup"><span data-stu-id="3e65f-107">site</span></span>
- <span data-ttu-id="3e65f-108">Liste</span><span class="sxs-lookup"><span data-stu-id="3e65f-108">list</span></span>
- <span data-ttu-id="3e65f-109">Kitaplığı</span><span class="sxs-lookup"><span data-stu-id="3e65f-109">library</span></span>

<span data-ttu-id="3e65f-110">Ayrıca, belirli özellikleri kullanan listeleri ve modern tarafından desteklenmeyen özelleştirmeleri yine otomatik olarak Klasik moda bırakılacak.</span><span class="sxs-lookup"><span data-stu-id="3e65f-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="3e65f-111">1 Nisan 2019, Kiracı düzeyi devre dışı bırakma işlemi başlayan opt dışında modern liste ve kitaplıkları Başlat ve 31 Mayıs 2019 devam.</span><span class="sxs-lookup"><span data-stu-id="3e65f-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="3e65f-112">Klasik mod Kiracı çevirme sonucu olan kitaplıkları ve listeleri otomatik olarak modern için kaydırılır.</span><span class="sxs-lookup"><span data-stu-id="3e65f-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="3e65f-113">Klasik mod gerekiyorsa lütfen daha fazla bilgi bakın [burada](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ve PnP Powershell talimatı seçenekleri ve bugün Klasik mod deneyimi kullanmak için kullanabileceğiniz araçları açıklar [burada](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) .</span><span class="sxs-lookup"><span data-stu-id="3e65f-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
