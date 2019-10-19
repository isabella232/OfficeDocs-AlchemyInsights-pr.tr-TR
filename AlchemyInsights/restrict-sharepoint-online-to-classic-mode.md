---
title: SharePoint Online'ı klasik moda yla sınırlandırın
ms.author: pebaum
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
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752088"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="cf635-102">SharePoint Online'ı klasik moda yla sınırlandırın</span><span class="sxs-lookup"><span data-stu-id="cf635-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="cf635-103">Bazı kuruluşlar hala Klasik mod deneyimi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="cf635-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="cf635-104">Parçalı düzeyde klasik modu kaldırma planları olmasa da, artık tüm bir kuruluşu (kiracı) listeler ve kitaplıklar için klasik modla sınırlamak mümkün değildir.</span><span class="sxs-lookup"><span data-stu-id="cf635-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="cf635-105">Yönetici, aşağıdaki düzeylerde sağladığımız parçalı devre dışı bırakma anahtarlarını kullanarak tek tek listeleri ve kitaplıkları klasik modda yönetmek için aşağıdaki seçeneklere sahip olacaktır:</span><span class="sxs-lookup"><span data-stu-id="cf635-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="cf635-106">site koleksiyonu</span><span class="sxs-lookup"><span data-stu-id="cf635-106">site collection</span></span>
- <span data-ttu-id="cf635-107">Site</span><span class="sxs-lookup"><span data-stu-id="cf635-107">site</span></span>
- <span data-ttu-id="cf635-108">Liste</span><span class="sxs-lookup"><span data-stu-id="cf635-108">list</span></span>
- <span data-ttu-id="cf635-109">Kitaplığı</span><span class="sxs-lookup"><span data-stu-id="cf635-109">library</span></span>

<span data-ttu-id="cf635-110">Ayrıca, belirli özellikleri ve modern tarafından desteklenmeyen özelleştirmeleri kullanan listeler otomatik olarak klasik moda geçilir.</span><span class="sxs-lookup"><span data-stu-id="cf635-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="cf635-111">1 Nisan 2019'dan itibaren, kiracı düzeyinde ki devre dışı bırakma süreci modern listeden ve kütüphanelerden 31 Mayıs 2019'a kadar başlayacak ve devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="cf635-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="cf635-112">Kiracı nın devre dışı bırakması sonucunda klasik modda olan listeler ve kütüphaneler otomatik olarak moderne kaydırılır.</span><span class="sxs-lookup"><span data-stu-id="cf635-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="cf635-113">Klasik mod aihtiyacınız varsa, lütfen [burada](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) daha fazla bilgi ve klasik mod deneyimini kullanmak için bugün kullanabileceğiniz seçenekleri ve araçları açıklayan PnP Powershell [talimatına](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) bakın.</span><span class="sxs-lookup"><span data-stu-id="cf635-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
