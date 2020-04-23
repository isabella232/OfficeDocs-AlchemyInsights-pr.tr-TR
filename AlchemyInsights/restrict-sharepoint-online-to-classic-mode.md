---
title: SharePoint Online'ı klasik moda yla sınırlandırın
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742489"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="518d9-102">SharePoint Online'ı klasik moda yla sınırlandırın</span><span class="sxs-lookup"><span data-stu-id="518d9-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="518d9-103">Bazı kuruluşlar hala Klasik mod deneyimi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="518d9-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="518d9-104">Parçalı düzeyde klasik modu kaldırma planları olmasa da, artık tüm bir kuruluşu (kiracı) listeler ve kitaplıklar için klasik modla sınırlamak mümkün değildir.</span><span class="sxs-lookup"><span data-stu-id="518d9-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="518d9-105">Yönetici, aşağıdaki düzeylerde sağladığımız parçalı devre dışı bırakma anahtarlarını kullanarak tek tek listeleri ve kitaplıkları klasik modda yönetmek için aşağıdaki seçeneklere sahip olacaktır:</span><span class="sxs-lookup"><span data-stu-id="518d9-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="518d9-106">site koleksiyonu</span><span class="sxs-lookup"><span data-stu-id="518d9-106">site collection</span></span>
- <span data-ttu-id="518d9-107">Site</span><span class="sxs-lookup"><span data-stu-id="518d9-107">site</span></span>
- <span data-ttu-id="518d9-108">Liste</span><span class="sxs-lookup"><span data-stu-id="518d9-108">list</span></span>
- <span data-ttu-id="518d9-109">Kitaplığı</span><span class="sxs-lookup"><span data-stu-id="518d9-109">library</span></span>

<span data-ttu-id="518d9-110">Ayrıca, belirli özellikleri ve modern tarafından desteklenmeyen özelleştirmeleri kullanan listeler otomatik olarak klasik moda geçilir.</span><span class="sxs-lookup"><span data-stu-id="518d9-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="518d9-111">1 Nisan 2019'dan itibaren, kiracı düzeyinde ki devre dışı bırakma süreci modern listeden ve kütüphanelerden 31 Mayıs 2019'a kadar başlayacak ve devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="518d9-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="518d9-112">Kiracı nın devre dışı bırakması sonucunda klasik modda olan listeler ve kütüphaneler otomatik olarak moderne kaydırılır.</span><span class="sxs-lookup"><span data-stu-id="518d9-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="518d9-113">Klasik mod aihtiyacınız varsa, lütfen [burada](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) daha fazla bilgi ve klasik mod deneyimini kullanmak için bugün kullanabileceğiniz seçenekleri ve araçları açıklayan PnP Powershell [talimatına](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) bakın.</span><span class="sxs-lookup"><span data-stu-id="518d9-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
