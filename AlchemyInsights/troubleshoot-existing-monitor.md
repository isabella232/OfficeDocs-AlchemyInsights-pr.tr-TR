---
title: Varolan monitörü sorun giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738588"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="2d8e0-102">Varolan bir monitörü sorun giderme</span><span class="sxs-lookup"><span data-stu-id="2d8e0-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="2d8e0-103">Bir monitörün sorun giderme için bu çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="2d8e0-104">**Monitörünüzün ekranını yenileyin:**</span><span class="sxs-lookup"><span data-stu-id="2d8e0-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="2d8e0-105">Aşağıdaki tuşlara aynı anda basın: Windows Tuşu + Ctrl + Shift + B. Bu, grafik sürücünüzle iletişimi yeniler.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="2d8e0-106">Monitörleriniz anlık yanıp sönecek ve birkaç saniye sonra geri gelecektir.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="2d8e0-107">**Sorun giderme monitör donanımı:**</span><span class="sxs-lookup"><span data-stu-id="2d8e0-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="2d8e0-108">Bilgisayarınızı monitörünüze bağlayan kabloyu çıkarın ve tekrar takın.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="2d8e0-109">Gerekli olmayan aygıtların bilgisayarınızdan (bağdaştırıcılar veya dock'lar gibi) bağlantısını kesin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="2d8e0-110">**Yakın zamanda bilgisayarınızda bir güncelleştirme yüklediyseniz, ekran sürücünüzgeri alabilirsiniz:**</span><span class="sxs-lookup"><span data-stu-id="2d8e0-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="2d8e0-111">**Başlat**, **aygıt yöneticisi**yazın ve sonuçlardan **Aygıt Yöneticisi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="2d8e0-112">Görüntü **bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınızı sağ tıklatın ve **Özellikleri**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="2d8e0-113">**Sürücü** sekmesine gidin ve **Geri Döndü Sürücüsü'nü**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="2d8e0-114">Not: Bu kullanılamıyorsa veya gri renkteyse, bir sonraki adıma geçmek için aşağıdaki seçeneklerden **Hayır'ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="2d8e0-115">Bu değişiklikler yürürlüğe girmeden önce bilgisayarınızı yeniden başlatmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="2d8e0-116">**Ekran sürücünüzün kaldırın ve yeniden yükleyin:**</span><span class="sxs-lookup"><span data-stu-id="2d8e0-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="2d8e0-117">**Başlat**, **aygıt yöneticisi**yazın ve sonuçlardan **Aygıt Yöneticisi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="2d8e0-118">Görüntü **bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınızı sağ tıklatın ve aygıtı **kaldır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="2d8e0-119">**Bu aygıtın sürücü yazılımını sil'in** yanındaki kutuyu seçin ve **Kaldır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="2d8e0-120">Not: Bu aşamada bilgisayarınızı yeniden başlatmanız istenebilir.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="2d8e0-121">Yeniden başlatmadan önce kalan yönergeleri yazdığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="2d8e0-122">Aygıt Yöneticisi'ni yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="2d8e0-123">Görüntü **bağdaştırıcıları** bölümünü genişletin, görüntü bağdaştırıcınıza sağ tıklayın ve **Sürücüyü Güncelleştir'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="2d8e0-124">**Sürücü yazılımını güncelleştirmek için otomatik olarak Ara'yı** seçin ve yükleme yönergelerini izleyin.</span><span class="sxs-lookup"><span data-stu-id="2d8e0-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>