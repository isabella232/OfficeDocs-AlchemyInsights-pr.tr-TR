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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516799"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="dd129-102">Gelen içerik arama/dışarı sonuç</span><span class="sxs-lookup"><span data-stu-id="dd129-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="dd129-103">Kur tarafından belirli bir yönetim ve tüm Yöneticiler grubuna Kurulmuyor, belirli uyumluluk güvenlik filtresi nedeniyle sorunlar ile içerik arama/herhangi veri döndürmek değil dışarı olabilir.</span><span class="sxs-lookup"><span data-stu-id="dd129-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="dd129-104">Bu sorunu gidermek için bu neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:</span><span class="sxs-lookup"><span data-stu-id="dd129-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="dd129-105">Güvenlik ve Uyumluluk Merkezi Powershell bağlanmak</span><span class="sxs-lookup"><span data-stu-id="dd129-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="dd129-106">Aşağıdaki commandlet'lerini çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="dd129-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="dd129-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="dd129-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="dd129-108">Get-ComplianceSecurityFilter-$org organizasyon</span><span class="sxs-lookup"><span data-stu-id="dd129-108">Get-ComplianceSecurityFilter -Organization $org</span></span>