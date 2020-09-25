---
title: eBulma dışarı aktarma aracı
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277945"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="26000-102">EBulma dışarı aktarma aracı yüklenemiyor veya çalıştırılamıyor misiniz?</span><span class="sxs-lookup"><span data-stu-id="26000-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="26000-103">Arama sonuçlarını indirmek için eBulma dışarı aktarma aracı 'nı yükleyemiyor veya çalıştıramıyorsanız, aşağıdakileri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="26000-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="26000-104">Kullandığınız bilgisayar bu önkoşulları karşılar:</span><span class="sxs-lookup"><span data-stu-id="26000-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="26000-105">Windows 7 ve sonraki sürümlerin 32 veya 64-bit sürümleri</span><span class="sxs-lookup"><span data-stu-id="26000-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="26000-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="26000-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="26000-107">Desteklenen bir tarayıcı:</span><span class="sxs-lookup"><span data-stu-id="26000-107">A supported browser:</span></span>

  - <span data-ttu-id="26000-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="26000-108">Microsoft Edge</span></span>

    <span data-ttu-id="26000-109">Veya</span><span class="sxs-lookup"><span data-stu-id="26000-109">Or</span></span>

  - <span data-ttu-id="26000-110">Internet Explorer 10 ve sonraki sürümleri</span><span class="sxs-lookup"><span data-stu-id="26000-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="26000-111">Google Chrome ve Mozilla Firefox gibi diğer tarayıcılar desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="26000-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="26000-112">Kuruluşunuz, Azure 'da \*\* \* . blob.Core.Windows.net\*\* (joker karakter, dışarı aktarma işiniz için benzersiz tanımlayıcıyı temsil eder) uç noktasına bağlanabilir.</span><span class="sxs-lookup"><span data-stu-id="26000-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="26000-113">Microsoft 365 güvenlik Uyumluluk Merkezi 'nde dışarı aktarma rolüne atanırsınız &amp; .</span><span class="sxs-lookup"><span data-stu-id="26000-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="26000-114">Varsayılan olarak bu rol yalnızca eBulma Yöneticisi rol grubuna atanır.</span><span class="sxs-lookup"><span data-stu-id="26000-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="26000-115">[EBulma Izinleri atama](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="26000-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="26000-116">Daha fazla bilgi için bkz: [Içerik arama sonuçlarını dışarı aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="26000-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="26000-117">100K posta kutularını dışarı aktarıyorsanız, dışarı aktarma sonuçlarını indirmek için aşağıdaki PowerShell 'i kullanmanız gerekir:  [100 ' den fazla posta kutusu 'ndan sonuçları dışarı aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="26000-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>