---
title: İçerik Arama Sonucu Yok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816868"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="69127-102">İçerik Arama/Dışarı Aktarma sonuçlarından sonuç yok</span><span class="sxs-lookup"><span data-stu-id="69127-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="69127-103">İçerik Arama/Dışarı Aktarma işlemiyle ilgili hiçbir veri döndürene sorunlar, belirli bir Yönetici tarafından kurulumu yapılan ve tüm Yöneticilere ile iletişim kurmadan dolayı belirli bir Uyumluluk Güvenlik Filtresi olabilir.</span><span class="sxs-lookup"><span data-stu-id="69127-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="69127-104">Bu sorunu çözmek için, soruna neden olacak herhangi bir Uyumluluk Güvenlik Filtresi olup olmadığını kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="69127-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="69127-105">Güvenlik ve Uyumluluk Merkezi Powershell'e bağlanma</span><span class="sxs-lookup"><span data-stu-id="69127-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="69127-106">Aşağıdaki komutlar çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="69127-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="69127-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="69127-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="69127-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="69127-108">Get-ComplianceSecurityFilter -Organization $org</span></span>