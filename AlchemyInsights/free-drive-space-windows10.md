---
title: Windows 10'da sürücü alanı boş bırak
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037952"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="adc34-102">Windows 10'da sürücü alanı boş bırak</span><span class="sxs-lookup"><span data-stu-id="adc34-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="adc34-103">Windows'da sürücü alanı için iki seçenek vardır:</span><span class="sxs-lookup"><span data-stu-id="adc34-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="adc34-104">Windows 10'da sürücü alanınız için boş alan sağlar.</span><span class="sxs-lookup"><span data-stu-id="adc34-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="adc34-105">Dış depolama cihazıyla Windows 10 güncelleştirmeleri için yer açın.</span><span class="sxs-lookup"><span data-stu-id="adc34-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="adc34-106">Disk Temizleme'yi kullandıktan sonra disk alanınız hala düşükse, Temp klasörünüz Microsoft Store tarafından kullanılan uygulama (.appx) dosyalarıyla hızla dolduruluyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="adc34-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="adc34-107">Bu sorunu çözmek için Mağaza'yı sıfırlayın, Mağaza önbelleğini temizleyin ve Windows Update sorun gidericisini çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="adc34-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="adc34-108">Bu adımlarla devammeden önce Microsoft Store'un kapalı olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="adc34-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="adc34-109">**1. Adım: Microsoft Store'u sıfırlama**</span><span class="sxs-lookup"><span data-stu-id="adc34-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="adc34-110">**Not** Bu, tercihleriniz ve oturum açma ayrıntıları da dahil olmak üzere cihaz üzerinde uygulama verilerini kalıcı olarak siler.</span><span class="sxs-lookup"><span data-stu-id="adc34-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="adc34-111">Başlangıç **Ayarları**  >  **Uygulamaları**  >  **uygulamaları**&  >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="adc34-112">Uygulama listesinde Microsoft Store'u bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="adc34-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="adc34-113">Gelişmiş **seçenekleri belirleyin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="adc34-114">Aşağı kaydırın ve **Sıfırla'yı seçin** ve sonra Sıfırlamayı **Onayla'yı seçin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="adc34-115">**2. Adım: Microsoft Store önbelleğini temizleme**</span><span class="sxs-lookup"><span data-stu-id="adc34-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="adc34-116">Çalıştır iletişim kutusunu açmak için Windows Logo Tuşu + R tuşlarına basın.</span><span class="sxs-lookup"><span data-stu-id="adc34-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="adc34-117">Arama wsreset.exe Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="adc34-118">Boş bir Komut İstemi penceresi açılır.</span><span class="sxs-lookup"><span data-stu-id="adc34-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="adc34-119">Yaklaşık 10 saniye sonra pencere kapanır ve Mağaza otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="adc34-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="adc34-120">**3. Adım: Windows Update'i sıfırlama**</span><span class="sxs-lookup"><span data-stu-id="adc34-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="adc34-121">Güvenlik **Sorunlarını**  >  **Gidermek**  >  **için Ayarlar &'ni**  >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="adc34-122">Aşağı kaydırın ve **listeden Windows Update'i** seçin ve sorun **gidericiyi çalıştır'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="adc34-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="adc34-123">Bilgisayarınızı yeniden başlatın ve sorunu hala yaşıyor olup olmadığınızı kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="adc34-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

