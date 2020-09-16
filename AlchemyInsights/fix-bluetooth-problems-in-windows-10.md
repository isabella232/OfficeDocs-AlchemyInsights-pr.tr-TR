---
title: Windows 10 ' da Bluetooth sorunlarını düzeltme
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730179"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="e14ea-102">Windows 10 ' da Bluetooth sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="e14ea-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="e14ea-103">Bluetooth simgesi eksikse veya Bluetooth etkinleştirilmemişse veya kapatılırsa, Bluetooth sorun gidericisini çalıştırmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e14ea-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="e14ea-104">[Sorun giderme ayarları 'Nı açın](ms-settings:troubleshoot), **Bluetooth** 'A tıklayarak **diğer sorunları bulun ve düzeltin**, **sorun gidericiyi çalıştırın**öğesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="e14ea-105">Bluetooth simgesini görmüyorsanız, ancak Bluetooth simge görüntüsü görüntülenir:</span><span class="sxs-lookup"><span data-stu-id="e14ea-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="e14ea-106">Aygıt Yöneticisi 'nde **Bluetooth**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="e14ea-107">Bluetooth bağdaştırıcı adını basılı tutun (veya sağ tıklayın) ve **Cihazı kaldır**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="e14ea-108">Windows cihazınızı kapatın, birkaç saniye bekleyin ve sonra tekrar açın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="e14ea-109">Windows sürücüyü yeniden yüklemeyi deneyecek.</span><span class="sxs-lookup"><span data-stu-id="e14ea-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="e14ea-110">En son Windows 10 güncelleştirmelerini yüklediyseniz veya Windows 10 ' a yükselttiyseniz, sürücü güncelleştirmelerini denetlemek isteyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e14ea-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="e14ea-111">Cihaz Yöneticisi 'nde **Bluetooth**'a tıklayın ve ardından Bluetooth bağdaştırıcısının adını ("radyo" sözcüğünü içerebilir) tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="e14ea-112">Bluetooth bağdaştırıcısını basılı tutun (veya sağ tıklayın) ve ardından **Update driver**  >  **güncelleştirilmiş sürücü yazılımı için otomatik olarak sürücü aramayı**Güncelleştir 'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="e14ea-113">Adımları izleyin ve **Kapat**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="e14ea-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="e14ea-114">Windows yeni bir Bluetooth sürücüsü bulamazsa, PC üreticisinin Web sitesini ziyaret edin ve buradan en son Bluetooth sürücüsünü indirin.</span><span class="sxs-lookup"><span data-stu-id="e14ea-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="e14ea-115">Sürücüyü indirdikten sonra **, sürücü**  >  **yazılımı için bilgisayarımı tara**'ya tıklayın sürücü  >  dosyalarının depolandığı konuma**göz atın** > ileri 'ye gidin ve **sonra**  >  **Next**yükleme adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="e14ea-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="e14ea-116">Güncelleştirilmiş sürücüyü yükledikten sonra makineyi yeniden başlatın ve bunun bağlantı sorununu düzeltip düzeltmeyeceğini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="e14ea-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="e14ea-117">Bluetooth sorunlarını giderme hakkında daha fazla bilgi için, Windows 10 ' da tüm makaleye bakın, [Bluetooth sorunlarını düzeltin](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="e14ea-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
