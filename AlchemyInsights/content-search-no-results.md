---
title: İçerik arama sonuç yok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680667"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="7f7af-102">Içerik arama/dışarı aktarma işleminden gelen sonuçlar yok</span><span class="sxs-lookup"><span data-stu-id="7f7af-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="7f7af-103">Içerik arama/dışarı aktarma ile ilgili sorunlar, belirli bir yönetici tarafından ayarlanmış olan ve tüm yöneticilerle iletişim kurmayabilir.</span><span class="sxs-lookup"><span data-stu-id="7f7af-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="7f7af-104">Bunu çözmek için, bu soruna neden olabilecek uyumluluk güvenlik filtreleri olup olmadığını denetleyin:</span><span class="sxs-lookup"><span data-stu-id="7f7af-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="7f7af-105">Güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanma</span><span class="sxs-lookup"><span data-stu-id="7f7af-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="7f7af-106">Aşağıdaki komutu çalıştırarak:</span><span class="sxs-lookup"><span data-stu-id="7f7af-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="7f7af-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="7f7af-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="7f7af-108">Get-Karmaşıısecurityfilter-kuruluş $org</span><span class="sxs-lookup"><span data-stu-id="7f7af-108">Get-ComplianceSecurityFilter -Organization $org</span></span>