---
title: eBulma içerirken oluşan hataları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676286"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="e514f-102">eBulma içerirken oluşan hataları giderme</span><span class="sxs-lookup"><span data-stu-id="e514f-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="e514f-103">eBulma 10 ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="e514f-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="e514f-104">Göz önünde bulundurarak en iyi yöntemlerden bazıları:</span><span class="sxs-lookup"><span data-stu-id="e514f-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="e514f-105">Tutma dağılımı durumunu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="e514f-105">Check the hold distribution status.</span></span>  <span data-ttu-id="e514f-106">Durum, Kapalı **(Beklemede) veya** **Kapalı (Beklemede)** ise, dağıtımın tamamlanması için beklemede bekleyin.</span><span class="sxs-lookup"><span data-stu-id="e514f-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="e514f-107">eBulma güncelleştirmelerini her işlemde ilkeyi tekrar tekrar güncelleştirmek yerine tek bir toplu istekte birleştirin.</span><span class="sxs-lookup"><span data-stu-id="e514f-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="e514f-108">Güvenlik Set-CaseHoldPolicy <policyname> Uyumluluk Merkezi Powershell'de -RetryDistribution'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="e514f-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="e514f-109">Ayrıntılar için güvenlik ve [Bağlan Merkezi PowerShell& e bakın.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="e514f-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="e514f-110">Bu ayarları denetleme adımları ve eBulma tutma sorunlarını azaltmaya ve çözmeye yönelik en iyi diğer yöntemler için bkz. [eBulma tutma hatalarını giderme.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="e514f-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="e514f-111">Sık karşılaşılan diğer eBulma sorunlarını giderme hakkında daha fazla bilgi için bkz. Yaygın eBulma sorunlarını araştırma, giderme [ve çözme.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="e514f-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
