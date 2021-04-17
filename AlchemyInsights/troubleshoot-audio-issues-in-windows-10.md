---
title: Windows 10'da ses sorunlarını giderme
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833311"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="d6ee0-102">Windows 10'da ses sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="d6ee0-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="d6ee0-103">**Ses sorun gidericisini çalıştırma**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="d6ee0-104">Sorun giderme [ayarlarını açın.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="d6ee0-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="d6ee0-105">Ses **Çalma Sorun**  >  **gidericisini çalıştır öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="d6ee0-106">**Varsayılan cihazı ayarlama**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-106">**Set the default device**</span></span>

<span data-ttu-id="d6ee0-107">USB veya HDMI kullanarak bir ses cihazına bağlanıyorsanız, bu cihazı varsayılan olarak ayarlamanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="d6ee0-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="d6ee0-108">Ses **Başlat**  >  **öğesini** açın ve sonuç **listesinden** **Ses'i veya Sistem seslerini** değiştir'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="d6ee0-109">Kayıttan **Yürütme sekmesinde** bir cihaz seçin, Varsayılanı **Ayarla'ya tıklayın** ve ardından Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="d6ee0-110">**Kabloları, ses düzeyini, hoparlörleri ve kulaklıkları kontrol edin**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="d6ee0-111">Gevşek kablo olup olmadığını kontrol edin ve doğru jaka bağlı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="d6ee0-112">Güç ve ses düzeylerinizi kontrol edin ve tüm ses denetimlerini yukarı doğru çevirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="d6ee0-113">Bazı hoparlörler ve uygulamaların kendi ses denetimleri vardır; Doğru düzeylerde olduğundan emin olmak için hepsini denetlemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="d6ee0-114">Farklı bir USB bağlantı noktası kullanarak bağlanmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="d6ee0-115">**Not:** Kulaklık takılıyken hoparlörlerin çalışmay olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="d6ee0-116">**Cihaz Yöneticisi'ni denetleme**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-116">**Check Device Manager**</span></span>

<span data-ttu-id="d6ee0-117">Sürücülerin güncel olduğundan emin olmak için:</span><span class="sxs-lookup"><span data-stu-id="d6ee0-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="d6ee0-118">Başlat **öğesini** seçin, **Cihaz Yöneticisi** yazın ve ardından sonuç **listesinden** Cihaz Yöneticisi'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="d6ee0-119">Ses, **video ve oyun kumandaları altında** ses kartınızı seçin, açın, Sürücü sekmesini **seçin** ve Sürücüyü **Güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="d6ee0-120">**Not:** Windows yeni bir sürücü bulamazsa cihaz üreticisinin web sitesinden bir sürücü bulun ve yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="d6ee0-121">**Sürücüyü yeniden yükleyin**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-121">**Reinstall the driver**</span></span>

<span data-ttu-id="d6ee0-122">Cihaz Yöneticisi aracılığıyla güncelleştire değilken üreticinin web sitesinde yeni bir sürücü bulamıyorsanız şu adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="d6ee0-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="d6ee0-123">Cihaz Yöneticisi'nde ses sürücüsüne sağ tıklayın (veya basılı tutun) ve Kaldır öğesini **seçin.**</span><span class="sxs-lookup"><span data-stu-id="d6ee0-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="d6ee0-124">Cihazınızı yeniden başlatın; Windows sürücüyü yeniden yüklemeyi dener.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="d6ee0-125">Sürücüyü yeniden yüklemek işe yaramadı mı? Windows ile birlikte gelen genel ses sürücüsünü kullanmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="d6ee0-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="d6ee0-126">Cihaz Yöneticisi'nde ses sürücüne sağ tıklayın (veya basılı tutun) > Sürücü yazılımını güncelleştir Sürücü yazılımı için bilgisayarıma göz at Bilgisayarımda bulunan cihaz sürücüleri listesinden seçmeme izin ver, Yüksek Tanımlı Ses Cihazı 'ı seçin, Sonraki'yi seçin ve yüklemek için yönergeleri  >    >  izleyin.  </span><span class="sxs-lookup"><span data-stu-id="d6ee0-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
