---
title: eBulma/İçerik Arama sonuçlarını dışarı aktarma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430298"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="0be7e-102">eBulma/İçerik Arama sonuçlarını dışarı aktarma</span><span class="sxs-lookup"><span data-stu-id="0be7e-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="0be7e-103">Arama sonuçlarınızı bir PST dosyasına (e-postadan) veya yerel Office belgelerine (SharePoint ve OneDrive İş sitelerinden) dışarı aktarmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="0be7e-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="0be7e-104">Öyleyse, şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="0be7e-104">If so, do the following:</span></span>

- <span data-ttu-id="0be7e-105">Hesabınıza dışarı aktarma için uygun izinlerin atandığı emin olun.</span><span class="sxs-lookup"><span data-stu-id="0be7e-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="0be7e-106">Daha fazla bilgi için bkz. [eBulma izni atama.](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="0be7e-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="0be7e-107">Bilgisayarınızın tüm önkoşullara uyan olduğundan [emin olun.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="0be7e-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="0be7e-108">Chrome gibi tüm tarayıcılar desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="0be7e-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="0be7e-109">İçerik Arama'dan dışarı aktarma: a.</span><span class="sxs-lookup"><span data-stu-id="0be7e-109">To export from a Content Search: a.</span></span> <span data-ttu-id="0be7e-110">Güvenlik Ve Uyumluluk [&'ne gidin](https://protection.office.com/contentsearch) ve Ara'ya **tıklayın** ve İçerik **arama'yı seçin.**</span><span class="sxs-lookup"><span data-stu-id="0be7e-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="0be7e-111">İçerik **arama sayfasında,** kaydedilmiş bir arama seçin.</span><span class="sxs-lookup"><span data-stu-id="0be7e-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="0be7e-112">b.</span><span class="sxs-lookup"><span data-stu-id="0be7e-112">b.</span></span> <span data-ttu-id="0be7e-113">Ayrıntılar bölmesinde, Sonuçları bilgisayara **aktar'ın altında Dışarı aktarmayı** **başlat'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="0be7e-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="0be7e-114">100.000'den fazla posta kutusunu dışarı aktarıyorsanız, dışarı aktarma sonuçlarını indirmek için PowerShell'i kullansanız iyi olur.</span><span class="sxs-lookup"><span data-stu-id="0be7e-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="0be7e-115">Daha fazla bilgi için bkz. [100.000'den fazla posta kutusundan sonuçları dışarı aktarma.](https://go.microsoft.com/fwlink/?linkid=2143861)</span><span class="sxs-lookup"><span data-stu-id="0be7e-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="0be7e-116">Daha fazla bilgi edinmek için, İçerik [Arama Sonuçlarını Dışarı Aktarma'ya bakın.](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="0be7e-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>