---
title: İçeriği arama sonucu yok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800666"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="37a67-102">Gelen içerik arama/dışarı sonuç</span><span class="sxs-lookup"><span data-stu-id="37a67-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="37a67-103">Kur tarafından belirli bir yönetim ve tüm Yöneticiler grubuna Kurulmuyor, belirli uyumluluk güvenlik filtresi nedeniyle sorunlar ile içerik arama/herhangi veri döndürmek değil dışarı olabilir.</span><span class="sxs-lookup"><span data-stu-id="37a67-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="37a67-104">Bu sorunu gidermek için bu neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:</span><span class="sxs-lookup"><span data-stu-id="37a67-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="37a67-105">Güvenlik ve Uyumluluk Merkezi Powershell bağlanmak</span><span class="sxs-lookup"><span data-stu-id="37a67-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="37a67-106">Aşağıdaki commandlet'lerini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="37a67-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="37a67-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="37a67-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="37a67-108">Get-ComplianceSecurityFilter-$org organizasyon</span><span class="sxs-lookup"><span data-stu-id="37a67-108">Get-ComplianceSecurityFilter -Organization $org</span></span>