---
title: Var olan monitörde sorun giderme
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690731"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="97d44-102">Var olan monitörde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="97d44-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="97d44-103">Monitörde sorun gidermek için bu çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="97d44-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="97d44-104">**Monitörünüzün görünümünü yenileyin:**</span><span class="sxs-lookup"><span data-stu-id="97d44-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="97d44-105">Aynı anda aşağıdaki tuşlara basın: Windows tuşu + CTRL + SHIFT + B. Bu, Grafik sürücünüzün iletişimini yenileyecektir.</span><span class="sxs-lookup"><span data-stu-id="97d44-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="97d44-106">Monitörleriniz anlık olarak yanıp sönecektir ve birkaç saniye sonra geri döner.</span><span class="sxs-lookup"><span data-stu-id="97d44-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="97d44-107">**Monitör donanımında sorun giderme:**</span><span class="sxs-lookup"><span data-stu-id="97d44-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="97d44-108">Bilgisayarınızı izleyicisine bağlayan kabloyu çıkarın ve takın.</span><span class="sxs-lookup"><span data-stu-id="97d44-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="97d44-109">Gerekli olmayan aygıtların bilgisayarınızdan (bağdaştırıcılar veya noktaları gibi) bağlantılarını kesin.</span><span class="sxs-lookup"><span data-stu-id="97d44-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="97d44-110">**Yakın zamanda bilgisayarınıza bir güncelleştirme yüklediyseniz, görüntü sürücünüzü geri alabilirsiniz:**</span><span class="sxs-lookup"><span data-stu-id="97d44-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="97d44-111">**Başlat**'ı seçin, **Cihaz Yöneticisi**yazın ve sonuçlardan **Cihaz Yöneticisi 'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="97d44-112">**Görüntü bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınızı sağ tıklatın ands **özellikleri**seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="97d44-113">**Sürücü** sekmesine gidin ve **sürücüye geri dön**öğesini seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="97d44-114">Not: Bu kullanılamaz veya gri görüntüleniyorsa, sonraki adıma geçmek için aşağıdaki seçeneklerden **Hayır** 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="97d44-115">Bu değişikliklerin yürürlüğe geçmeden bilgisayarınızı yeniden başlatmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="97d44-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="97d44-116">**Görüntü sürücünüzü kaldırın ve yeniden yükleyin:**</span><span class="sxs-lookup"><span data-stu-id="97d44-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="97d44-117">**Başlat**'ı seçin, **Cihaz Yöneticisi**yazın ve sonuçlardan **Cihaz Yöneticisi 'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="97d44-118">**Görüntü bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınızı sağ tıklatın ands **Cihazı kaldır**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="97d44-119">**Bu cihaz için sürücü yazılımını sil** 'in yanındaki kutuyu seçin ve **Kaldır**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="97d44-120">Not: Bu aşamada bilgisayarınızı yeniden başlatmanız istenebilir.</span><span class="sxs-lookup"><span data-stu-id="97d44-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="97d44-121">Yeniden başlatmadan önce kalan yönergeleri yazdığınızdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="97d44-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="97d44-122">Cihaz Yöneticisi 'Ni yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="97d44-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="97d44-123">**Görüntü bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınızı sağ tıklatın ve **Sürücüyü Güncelleştir**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="97d44-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="97d44-124">**Sürücü yazılımını Güncelleştir için otomatik olarak ara** öğesini seçin ve yükleme yönergelerini izleyin.</span><span class="sxs-lookup"><span data-stu-id="97d44-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>