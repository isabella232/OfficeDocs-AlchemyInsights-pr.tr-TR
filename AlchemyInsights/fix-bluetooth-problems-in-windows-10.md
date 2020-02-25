---
title: Windows 10'daki Bluetooth sorunlarını düzeltme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268713"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="23a9f-102">Windows 10'daki Bluetooth sorunlarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="23a9f-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="23a9f-103">Bluetooth simgesi eksikse veya Bluetooth açılamaz veya kapatılamazsa, Bluetooth sorun gidericisini çalıştırmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="23a9f-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="23a9f-104">[Sorun Giderme ayarlarını açın,](ms-settings:troubleshoot) **Bluetooth'u** tıklatın **ve diğer sorunları düzeltin,** **sorun gidericiçalıştır'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="23a9f-105">Bluetooth simgesini görmüyorsanız, ancak Bluetooth Aygıt Yöneticisi'nde görünür:</span><span class="sxs-lookup"><span data-stu-id="23a9f-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="23a9f-106">Aygıt Yöneticisi'nde **Bluetooth'u**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="23a9f-107">Bluetooth bağdaştırıcısının adını basılı tutun ve basılı tutun ve **Aygıtı Kaldır'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="23a9f-108">Windows aygıtınızı kapatın, birkaç saniye bekleyin ve sonra tekrar açın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="23a9f-109">Windows sürücüyü yeniden yüklemeyi dener.</span><span class="sxs-lookup"><span data-stu-id="23a9f-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="23a9f-110">Yakın zamanda Windows 10 güncelleştirmelerini yüklediyseniz veya Windows 10'a yükselttiyseniz, sürücü güncelleştirmelerini denetlemek isteyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="23a9f-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="23a9f-111">Aygıt Yöneticisi'nde **Bluetooth'u**tıklatın ve ardından Bluetooth bağdaştırıcı adını tıklatın ("radyo" sözcüğü ne eklenebilir).</span><span class="sxs-lookup"><span data-stu-id="23a9f-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="23a9f-112">Bluetooth bağdaştırıcısını basılı tutun ve basılı tutun (veya sağ tıklatın) ve**ardından güncelleştirilmiş sürücü yazılımı için**sürücü > aramasını otomatik olarak **güncelleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="23a9f-113">Adımları izleyin ve ardından **Kapat'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="23a9f-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="23a9f-114">Windows yeni bir Bluetooth sürücüsü bulamazsa, BILGISAYAR üreticisinin web sitesini ziyaret edin ve en son Bluetooth sürücüsünü buradan indirin.</span><span class="sxs-lookup"><span data-stu-id="23a9f-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="23a9f-115">İndirdikten sonra, sürücü yazılımı\*\*\*\*  > **için bilgisayarıma Göz at'ı** \*\*\*\* > tıklatın Sürücü dosyalarının depolandığı konuma göz atın > **Tamam** > **Sonraki**ve yükleme adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="23a9f-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="23a9f-116">Güncelleştirilmiş sürücüyü yükledikten sonra makineyi yeniden başlatın ve bağlantı sorununu giderip düzeltmediğini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="23a9f-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="23a9f-117">Bluetooth sorunlarını nasıl gidereceğimiz hakkında daha fazla bilgi için lütfen tam makaleye bakın, [Windows 10'daki Bluetooth sorunlarını düzeltin.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="23a9f-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
