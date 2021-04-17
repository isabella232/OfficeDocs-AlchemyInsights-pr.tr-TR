---
title: Mevcut monitörde sorun giderme
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824599"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="60192-102">Mevcut monitörde sorun giderme</span><span class="sxs-lookup"><span data-stu-id="60192-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="60192-103">Monitörle ilgili sorunları gidermek için aşağıdaki çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="60192-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="60192-104">**Monitör ekranınızı yenileyin:**</span><span class="sxs-lookup"><span data-stu-id="60192-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="60192-105">Şu tuşlara aynı anda basın: Windows Tuşu + Ctrl + Shift + B. Bu, grafik sürücüyle iletişimi yeniler.</span><span class="sxs-lookup"><span data-stu-id="60192-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="60192-106">Monitörler kısa bir süre yanıp söner ve birkaç saniye sonra geri döner.</span><span class="sxs-lookup"><span data-stu-id="60192-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="60192-107">**Monitör donanımıyla ilgili sorunları giderme:**</span><span class="sxs-lookup"><span data-stu-id="60192-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="60192-108">Bilgisayarınızı monitörünüze bağlayan kabloyu çıkarın ve yeniden takın.</span><span class="sxs-lookup"><span data-stu-id="60192-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="60192-109">Bilgisayarınızdan (bağdaştırıcılar veya takma cihazları gibi) gerekli olmayan cihazların bağlantısını kesin.</span><span class="sxs-lookup"><span data-stu-id="60192-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="60192-110">**Yakın zamanda bilgisayarınıza bir güncelleştirme yüklemişsiniz, ekran sürücülerinizi geri yükleyebilirsiniz:**</span><span class="sxs-lookup"><span data-stu-id="60192-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="60192-111">Başlat **öğesini** seçin, **cihaz yöneticisi yazın** ve **sonuçlardan Cihaz Yöneticisi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="60192-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="60192-112">Görüntü **bağdaştırıcıları bölümünü genişletin,** ekran bağdaştırıcınıza sağ tıklayın ve Özellikler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="60192-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="60192-113">Sürücü sekmesine **gidin** ve Sürücüye Geri **Dön öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="60192-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="60192-114">Not: Bu seçenek kullanılamıyorsa veya gri renkte  gösterilirse, sonraki adıma taşımak için aşağıdaki seçeneklerden Hayır'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="60192-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="60192-115">Bu değişikliklerin etkili olması için bilgisayarınızı yeniden başlatmanız gerekiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="60192-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="60192-116">**Ekran sürücülerinizi kaldırın ve yeniden yükleyin:**</span><span class="sxs-lookup"><span data-stu-id="60192-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="60192-117">Başlat **öğesini** seçin, **cihaz yöneticisi yazın** ve **sonuçlardan Cihaz Yöneticisi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="60192-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="60192-118">Görüntü **bağdaştırıcıları bölümünü genişletin,** ekran bağdaştırıcınıza sağ tıklayın ve Cihazı **kaldır'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="60192-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="60192-119">Bu cihaz için sürücü yazılımını **sil'in yanındaki kutuyu seçin ve kaldır'ı** **seçin.**</span><span class="sxs-lookup"><span data-stu-id="60192-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="60192-120">Not: Bu aşamada bilgisayarınızı yeniden başlatmanız istenebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="60192-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="60192-121">Yeniden başlatmadan önce kalan yönergeleri not edin.</span><span class="sxs-lookup"><span data-stu-id="60192-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="60192-122">Cihaz Yöneticisi'ni yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="60192-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="60192-123">Görüntü **bağdaştırıcıları bölümünü genişletin,** ekran bağdaştırıcınıza sağ tıklayın ve Sürücüyü **Güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="60192-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="60192-124">Sürücü **yazılımını otomatik olarak güncelleştir'i seçin** ve yükleme yönergelerini izleyin.</span><span class="sxs-lookup"><span data-stu-id="60192-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>