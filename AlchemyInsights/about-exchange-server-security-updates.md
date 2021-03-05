---
title: Exchange Server Güvenlik güncelleştirmeleri hakkında
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482984"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="5f042-102">Exchange Server Güvenlik güncelleştirmeleri hakkında</span><span class="sxs-lookup"><span data-stu-id="5f042-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="5f042-103">Microsoft, Exchange Server şirket içi için bir dizi kritik güvenlik güncelleştirmesi yayımladı.</span><span class="sxs-lookup"><span data-stu-id="5f042-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="5f042-104">Etkilenen sunucu sürümleri Exchange Server 2010, 2013, 2016 ve 2019'un tüm güncelleştirme düzeyleridir.</span><span class="sxs-lookup"><span data-stu-id="5f042-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="5f042-105">Exchange Online etkilenmez, ancak Karma yapılandırmadan dolayı bazı şirket içi Exchange sunucularınız varsa, bunlar potansiyel olarak zayıf olabilir.</span><span class="sxs-lookup"><span data-stu-id="5f042-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="5f042-106">Şirket içi sunucularınızı güncelleştirmek için, exchange'in en azından aşağıdaki sürümlerinin çalışıyor olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="5f042-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="5f042-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="5f042-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="5f042-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="5f042-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="5f042-109">Exchange Server 2016 CU 19 veya CU 18</span><span class="sxs-lookup"><span data-stu-id="5f042-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="5f042-110">Exchange Server 2019 CU 8 veya CU 7</span><span class="sxs-lookup"><span data-stu-id="5f042-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="5f042-111">Düzeltmelerin konumu için lütfen şu duyuruya bakın: [Yayınlandı: Mart 2021 Exchange Server Güvenlik Güncelleştirmeleri](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="5f042-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="5f042-112">**Önemli notlar:**</span><span class="sxs-lookup"><span data-stu-id="5f042-112">**Important notes:**</span></span>

<span data-ttu-id="5f042-113">Yukarıdaki listede olduğu gibi, şirket içi sunucularınız gerekli Exchange sürümlerini çalıştırmayacaksa, güncelleştirmelerin yüklenmesi çalışmayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5f042-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="5f042-114">Güncelleştirmeleri el ile yüklüyorsanız, önemli bilgiler için lütfen güncelleştirme KB makalelerinin "Bilinen sorunlar" bölümünü okuyun.</span><span class="sxs-lookup"><span data-stu-id="5f042-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="5f042-115">Güvenlik güncelleştirmeleri yükseltilmiş CMD/PowerShell isteminden çalıştır must bekli!</span><span class="sxs-lookup"><span data-stu-id="5f042-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
