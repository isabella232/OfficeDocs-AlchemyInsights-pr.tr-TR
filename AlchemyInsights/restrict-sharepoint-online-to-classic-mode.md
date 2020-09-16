---
title: SharePoint Online 'ı klasik moda kısıtlama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751443"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="96ebd-102">SharePoint Online 'ı klasik moda kısıtlama</span><span class="sxs-lookup"><span data-stu-id="96ebd-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="96ebd-103">Bazı kuruluşlar için klasik mod deneyimi gerekmektedir.</span><span class="sxs-lookup"><span data-stu-id="96ebd-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="96ebd-104">Klasik modu parçalı bir düzeyde kaldırmak için, artık bir organizasyonun (kiracı), listeler ve kitaplıklar için klasik mod ile sınırlanması mümkün değildir.</span><span class="sxs-lookup"><span data-stu-id="96ebd-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="96ebd-105">Yönetici, aşağıdaki düzeylerde sağladığımız parçalı geri çevirme anahtarlarını kullanarak tek tek listeleri ve kitaplıkları Klasik modda yönetmek için aşağıdaki seçeneklere sahiptir:</span><span class="sxs-lookup"><span data-stu-id="96ebd-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="96ebd-106">Site koleksiyonu</span><span class="sxs-lookup"><span data-stu-id="96ebd-106">site collection</span></span>
- <span data-ttu-id="96ebd-107">bölge</span><span class="sxs-lookup"><span data-stu-id="96ebd-107">site</span></span>
- <span data-ttu-id="96ebd-108">listeniz</span><span class="sxs-lookup"><span data-stu-id="96ebd-108">list</span></span>
- <span data-ttu-id="96ebd-109">Kitaplığı</span><span class="sxs-lookup"><span data-stu-id="96ebd-109">library</span></span>

<span data-ttu-id="96ebd-110">Ayrıca, çağdaş tarafından desteklenmeyen bazı özellikleri ve özelleştirmeleri kullanan listeler yine de otomatik olarak klasik moda dönüştürülür.</span><span class="sxs-lookup"><span data-stu-id="96ebd-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="96ebd-111">1 Nisan 2019, kiracı düzeyini devre dışı bırakma süreci modern listeden geri çevirmeye devam eder ve kitaplıklar 31 Mayıs 2019 ile başlayacak ve devam edecektir.</span><span class="sxs-lookup"><span data-stu-id="96ebd-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="96ebd-112">Kiracı geri çevirme sonucunda klasik moddaki listeler ve kitaplıklar otomatik olarak modern olarak kaydırılacaktır.</span><span class="sxs-lookup"><span data-stu-id="96ebd-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="96ebd-113">Klasik mod gerekliyse, klasik mod deneyimini kullanmak için bugün kullanabileceğiniz seçenekleri ve araçları [açıklayan daha](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) fazla bilgi için [buraya](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) bakın.</span><span class="sxs-lookup"><span data-stu-id="96ebd-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
