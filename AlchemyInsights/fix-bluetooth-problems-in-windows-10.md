---
title: Windows 10'da Bluetooth sorunlarını düzeltme
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812952"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="2e7e2-102">Windows 10'da Bluetooth sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="2e7e2-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="2e7e2-103">Bluetooth simgesi yoksa veya Bluetooth açık ya da kapalı olarak yoksa Bluetooth sorun gidericisini çalıştırmanız iyi olabilir.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="2e7e2-104">[Sorun giderme ayarlarını açın, Diğer](ms-settings:troubleshoot)sorunları bul ve **düzelt'in altında Bluetooth'a tıklayın,** Sorun **gidericiyi çalıştır 'a tıklayın.** </span><span class="sxs-lookup"><span data-stu-id="2e7e2-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="2e7e2-105">Bluetooth simgesini görmüyorsanız ancak Cihaz Yöneticisi'nde Bluetooth görüntü görünüyorsa:</span><span class="sxs-lookup"><span data-stu-id="2e7e2-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="2e7e2-106">Cihaz Yöneticisi'nde Bluetooth 'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="2e7e2-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="2e7e2-107">Bluetooth bağdaştırıcısı adına basılı tutun (veya sağ tıklayın) ve Cihazı **kaldır'a tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="2e7e2-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="2e7e2-108">Windows cihazınızı kapatın, birkaç saniye bekleyin ve sonra yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="2e7e2-109">Windows sürücüyü yeniden yüklemeyi dener.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="2e7e2-110">Yakın zamanda Windows 10 güncelleştirmelerini yüklemiş veya Windows 10'a yükselttiysanız, sürücü güncelleştirmelerini denetlemeniz iyi olabilir:</span><span class="sxs-lookup"><span data-stu-id="2e7e2-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="2e7e2-111">Cihaz Yöneticisi'nde **Bluetooth'a** tıklayın ve ardından Bluetooth bağdaştırıcısının adına ("radyo" sözcüğüyle olabilir) tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="2e7e2-112">Bluetooth bağdaştırıcısını basılı tutun (veya sağ tıklayın) ve ardından Sürücüyü güncelleştir Güncel sürücü **yazılımını** otomatik olarak ara  >  **'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="2e7e2-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="2e7e2-113">Adımları izleyin, ardından Kapat'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="2e7e2-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="2e7e2-114">Windows yeni bir Bluetooth sürücüsü bulamazsa bilgisayar üreticisinin web sitesini ziyaret edin ve en yeni Bluetooth sürücüsünü buradan indirin.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="2e7e2-115">İndirdikten sonra Sürücüyü güncelleştir Sürücü yazılımını bulmak için bilgisayarıma gözat Sürücü dosyalarının depolandığı konuma göz at'a tıklayın > Ardından, yüklemek  >    >   için   >  adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="2e7e2-116">Güncelleştirilmiş sürücüyü yükledikten sonra, makineyi yeniden başlatın ve bağlantı sorununa bir düzeltmenin olup olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="2e7e2-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="2e7e2-117">Bluetooth sorunlarını giderme hakkında daha fazla ayrıntı için lütfen [Windows 10'da Bluetooth sorunlarını giderme makalenin tamamını okuyun.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="2e7e2-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
