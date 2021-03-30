---
title: Gece ışığı ekran ayarıyla ilgili yardım
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405184"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="75c78-102">Gece ışığı ekran ayarıyla ilgili yardım</span><span class="sxs-lookup"><span data-stu-id="75c78-102">Help with the night light display setting</span></span>

<span data-ttu-id="75c78-103">Windows 10'da gece saati görüntüleme ayarları hakkında daha fazla bilgi edinmek için bkz. [Ekranınızı gece için ayarlama.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="75c78-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="75c78-104">Ayarlar'da gece ışığı seçenekleri gri görüntüleniyorsa ekran sürücüne bakın:</span><span class="sxs-lookup"><span data-stu-id="75c78-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="75c78-105">Görev çubuğunuzda arama kutusuna tıklayın ve **Cihaz** Yöneticisi yazın ve ardından arama sonuçlarında **Cihaz** Yöneticisi'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="75c78-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="75c78-106">Görüntü **bağdaştırıcılarını genişletin.**</span><span class="sxs-lookup"><span data-stu-id="75c78-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="75c78-107">Cihazınız DisplayLink sürücüsü veya Temel Ekran sürücüsü kullanıyorsa gece ışığı özelliği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="75c78-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="75c78-108">Gece ışığı özelliği en son grafik teknolojisini kullanır, bu nedenle ekran sürücünizi güncelleştirmeniz gerekir:</span><span class="sxs-lookup"><span data-stu-id="75c78-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="75c78-109">Güvenlik Windows Update'in **Güncelleştirmeleri**  >  **Denetleme'ye**  >  **& Ayarlar**  >  **Güncelleştirmesi'ne**  >  **gidip güncelleştirmeleri denetleme.**</span><span class="sxs-lookup"><span data-stu-id="75c78-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="75c78-110">VEYA</span><span class="sxs-lookup"><span data-stu-id="75c78-110">OR</span></span>

- <span data-ttu-id="75c78-111">En son görüntü sürücülerini el ile indirmek ve yüklemek için donanım üreticinizin destek web sitesini ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="75c78-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="75c78-112">Kayıt defterinde gece ışığını sıfırlama</span><span class="sxs-lookup"><span data-stu-id="75c78-112">Reset night light in the registry</span></span>

<span data-ttu-id="75c78-113">Ekran sürücü güncelleştirmeyi çalışmıyorsa kayıt defterinde gece ışığını sıfırlamanız gerekiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="75c78-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="75c78-114">**Dikkat:** Bu sorun giderme adımı yalnızca ileri düzey kullanıcılar için önerilir.</span><span class="sxs-lookup"><span data-stu-id="75c78-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="75c78-115">Kayıt defterinde yanlış bir değişiklik olursa, ciddi sorunlar oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="75c78-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="75c78-116">Ek koruma için, değişiklik yapmadan önce kayıt defterini yedeklenin, böylece sorun oluşursa geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="75c78-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="75c78-117">Arama kutusuna **regedit yazın ve ardından** arama sonuçlarında **Kayıt Defteri Düzenleyicisi'ni** seçin.</span><span class="sxs-lookup"><span data-stu-id="75c78-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="75c78-118">Aşağıdaki kayıt defteri anahtarına gidin:</span><span class="sxs-lookup"><span data-stu-id="75c78-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="75c78-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="75c78-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="75c78-120">Aşağıdaki alt anahtarı dışarı aktarın ve ardından silin:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="75c78-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="75c78-121">Şu alt anahtarı dışarı aktarın ve ardından silin:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="75c78-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="75c78-122">Windows'u yeniden başlatın ve gece ışığı seçeneklerinin kullanılabilir olup olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="75c78-122">Restart Windows and verify if the night light options are available.</span></span>


