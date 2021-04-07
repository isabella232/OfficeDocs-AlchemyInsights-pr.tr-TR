---
title: Windows 10’da sürücüde yer açma
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505376"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="26845-102">Windows 10’da sürücüde yer açma</span><span class="sxs-lookup"><span data-stu-id="26845-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="26845-103">Windows’ta sürücüde yer açmak için iki seçenek vardır:</span><span class="sxs-lookup"><span data-stu-id="26845-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="26845-104">Windows 10’da sürücüde yer açın.</span><span class="sxs-lookup"><span data-stu-id="26845-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="26845-105">Dış depolama cihazı kullanarak Windows 10 güncelleştirmeleri için yer açın.</span><span class="sxs-lookup"><span data-stu-id="26845-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="26845-106">Disk Temizleme aracını kullandıktan sonra disk alanınız hala yetersizse, Temp klasörünüz Microsoft Store tarafından kullanılan uygulama (.appx) dosyalarıyla hızlı bir şekilde doluyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="26845-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="26845-107">Bu sorunu çözmek için, Microsoft Store’u sıfırlayın, Microsoft Store önbelleğini temizleyin ve ardından Windows Update sorun gidericisini çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="26845-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="26845-108">Bu adımlara geçmeden önce Microsoft Store’un kapalı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="26845-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="26845-109">**1. Adım: Microsoft Store’u sıfırlayın**</span><span class="sxs-lookup"><span data-stu-id="26845-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="26845-110">**Not** Bu işlem, tercihleriniz veya oturum açma bilgileriniz dahil cihazdaki uygulama verilerini kalıcı olarak siler.</span><span class="sxs-lookup"><span data-stu-id="26845-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="26845-111">**Başlat** > **Ayarlar** > **Uygulamalar** > **Uygulamalar ve özellikleri**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="26845-112">Uygulamalar listesinde Microsoft Store’u bularak seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="26845-113">**Gelişmiş seçenekler**’i seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="26845-114">Aşağı kaydırın, **Sıfırla**’yı ve ardından **Sıfırlamayı Onayla** yı seçin. </span><span class="sxs-lookup"><span data-stu-id="26845-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="26845-115">**2. Adım: Microsoft Store önbelleğini temizleyin**</span><span class="sxs-lookup"><span data-stu-id="26845-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="26845-116">Windows logo tuşu + R tuşlarına basarak Çalıştır iletişim kutusunu açın.</span><span class="sxs-lookup"><span data-stu-id="26845-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="26845-117">Kutuya wsreset.exe yazın ve **Tamam**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="26845-118">Boş bir Komut İstemi penceresi açılır.</span><span class="sxs-lookup"><span data-stu-id="26845-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="26845-119">Yaklaşık 10 saniye sonra pencere kapanır ve Microsoft Store otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="26845-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="26845-120">**3. Adım: Windows Update’i sıfırlayın**</span><span class="sxs-lookup"><span data-stu-id="26845-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="26845-121">**Başlat** > **Ayarlar** > **Güncelleştirme ve Güvenlik** > **Sorun giderme**’yi seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="26845-122">Aşağı kaydırın ve listeden **Windows Update**’i seçin ve **Sorun gidericiyi çalıştır**’ı seçin.</span><span class="sxs-lookup"><span data-stu-id="26845-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="26845-123">Bilgisayarınızı yeniden başlatın ve sorunla karşılaşmaya devam edip etmediğinizi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="26845-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

