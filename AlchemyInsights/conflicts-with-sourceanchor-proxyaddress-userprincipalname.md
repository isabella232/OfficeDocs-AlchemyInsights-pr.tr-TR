---
title: SourceAnchor, ProxyAddress, UserPrincipalName ile çakışmalar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198577"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="ccef5-102">SourceAnchor, ProxyAddress, UserPrincipalName ile çakışmalar</span><span class="sxs-lookup"><span data-stu-id="ccef5-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="ccef5-103">"Dizininizde aynı ProxyAddress veya UserPrincipalName'e sahip eşitlenmiş bir nesne var" gibi bir eşitleme sırasında hatalar alırsanız, [bkz.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)</span><span class="sxs-lookup"><span data-stu-id="ccef5-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="ccef5-104">Ayrıca, yinelenen öznitelik esnekliği etkinleştirmeyi düşünün.</span><span class="sxs-lookup"><span data-stu-id="ccef5-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="ccef5-105">Daha fazla bilgi için [kimlik eşitlemesi ve yinelenen öznitelik esnekliğine](https://aka.ms/duplicateattributeresiliency)bakın.</span><span class="sxs-lookup"><span data-stu-id="ccef5-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>