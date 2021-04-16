---
title: eBulma dışarı aktarma aracı
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814608"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="f381b-102">eBulma Dışarı Aktarma Aracı'nı yükleye mi çalıştırasınız veya çalıştırasınız?</span><span class="sxs-lookup"><span data-stu-id="f381b-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="f381b-103">Arama sonuçlarını indirmek için eBulma Dışarı Aktarma Aracı'nı yükleye değil de çalıştırasanız, aşağıdaki kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="f381b-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="f381b-104">Kullanmakta olduğunuz bilgisayar şu önk önkulları karşılar:</span><span class="sxs-lookup"><span data-stu-id="f381b-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="f381b-105">Windows 7 ve sonraki sürümlerin 32 veya 64 bit sürümleri</span><span class="sxs-lookup"><span data-stu-id="f381b-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="f381b-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="f381b-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="f381b-107">Desteklenen bir tarayıcı:</span><span class="sxs-lookup"><span data-stu-id="f381b-107">A supported browser:</span></span>

  - <span data-ttu-id="f381b-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f381b-108">Microsoft Edge</span></span>

    <span data-ttu-id="f381b-109">Veya</span><span class="sxs-lookup"><span data-stu-id="f381b-109">Or</span></span>

  - <span data-ttu-id="f381b-110">Internet Explorer 10 ve sonraki sürümleri</span><span class="sxs-lookup"><span data-stu-id="f381b-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="f381b-111">Google Chrome ve Mozilla Firefox gibi diğer tarayıcılar desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="f381b-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="f381b-112">Organizasyonunız Azure'daki **\* .blob.core.windows.net** uç noktasına bağlanabilirsiniz (joker karakter, dışarı aktarma işinin benzersiz bir tanımlayıcısını temsil eder).</span><span class="sxs-lookup"><span data-stu-id="f381b-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="f381b-113">Microsoft 365 Güvenlik Uyumluluk Merkezi'nde Dışarı Aktarma &amp; rolüne atandık.</span><span class="sxs-lookup"><span data-stu-id="f381b-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="f381b-114">Varsayılan olarak, bu rol yalnızca eBulma Yöneticisi rol grubuna atanır.</span><span class="sxs-lookup"><span data-stu-id="f381b-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="f381b-115">Bkz. [eBulma izinleri atama.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="f381b-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="f381b-116">Daha fazla bilgi için bkz. [İçerik Arama sonuçlarını dışarı aktarma.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="f381b-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="f381b-117">100.000'den fazla posta kutusunu dışarı aktarıyorsanız, Sonuçları dışarı aktarma:  [100.000'den](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)fazla posta kutusundan sonuçları dışarı aktarma.</span><span class="sxs-lookup"><span data-stu-id="f381b-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>