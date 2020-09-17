---
title: Project Online salt okunur durumda
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801672"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="c1d19-102">Project Online salt okunur durumda</span><span class="sxs-lookup"><span data-stu-id="c1d19-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="c1d19-103">Project Online 'ın salt okunur duruma geçebileceği üç yaygın nedeni vardır:</span><span class="sxs-lookup"><span data-stu-id="c1d19-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="c1d19-104">Kuruluşların yalnızca Project Online Essentials lisansları vardır.</span><span class="sxs-lookup"><span data-stu-id="c1d19-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="c1d19-105">Bu, sitenin canlı kalmasını sağlamak için yeterli değildir ve sonunda da gerekecektir.</span><span class="sxs-lookup"><span data-stu-id="c1d19-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="c1d19-106">Siteyi salt okunur duruma yerleştirdik, böylece Yöneticiler bir şeyin yanlış olduğunu bilir ve doğru lisansları bulabilir.</span><span class="sxs-lookup"><span data-stu-id="c1d19-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="c1d19-107">Yöneticilerin Project Online Professional ve/veya Premium Lisansı eklemesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="c1d19-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="c1d19-108">Site bu noktada salt okunur olacaktır.</span><span class="sxs-lookup"><span data-stu-id="c1d19-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="c1d19-109">Daha fazla bilgi için bkz [.](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)</span><span class="sxs-lookup"><span data-stu-id="c1d19-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="c1d19-110">Atanan kotaya ulaşıldı.</span><span class="sxs-lookup"><span data-stu-id="c1d19-110">Assigned quota has been reached.</span></span> <span data-ttu-id="c1d19-111">Daha fazla bilgi için [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c1d19-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="c1d19-112">Ayrıntı belirleme raporlaması kota kullanımının nasıl etkileyebileceğini görmek için [Project Online 'daki zaman aşamalı raporlama verilerinin toplu rapor toplamasını](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="c1d19-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="c1d19-113">Salt okunur, bakım sırasında oluşabilen bir geçici koşul olabilir.</span><span class="sxs-lookup"><span data-stu-id="c1d19-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="c1d19-114">Çoğu bakım müşterilerimizden da fark etmeyecektir, ancak bu, genellikle salt okunur olan kısa dönemlerin olduğu zamanlar olur.</span><span class="sxs-lookup"><span data-stu-id="c1d19-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
