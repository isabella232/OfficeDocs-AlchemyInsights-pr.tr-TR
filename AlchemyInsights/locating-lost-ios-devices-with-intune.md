---
title: Kayıp iOS aygıtlarını Intune ile bulma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440432"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="d04b5-102">Kayıp iOS aygıtlarını Intune ile bulma</span><span class="sxs-lookup"><span data-stu-id="d04b5-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="d04b5-103">iOS aygıtında kayıp modu etkinleştirmek, yöneticinin kilit ekranında bir ileti ve iletişim telefonu numarasının görüntülenmesine olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="d04b5-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="d04b5-104">Kayıp modu etkinleştirildikten sonra yönetici, aygıtın fiziksel konumunu belirlemek için Cihazı Bul eylemini kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="d04b5-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="d04b5-105">Intune'daki Cihazı Bul eylemi, belirli bir aygıtın konumunu haritada göstermek için iOS aygıtlarıyla birlikte çalışır.</span><span class="sxs-lookup"><span data-stu-id="d04b5-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="d04b5-106">Bu eylemi kullanmak için iOS aygıtının aşağıdakilerde yer alabını gerektirir:</span><span class="sxs-lookup"><span data-stu-id="d04b5-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="d04b5-107">Denetlenen mod</span><span class="sxs-lookup"><span data-stu-id="d04b5-107">Supervised mode</span></span>
- <span data-ttu-id="d04b5-108">Kayıp mod</span><span class="sxs-lookup"><span data-stu-id="d04b5-108">Lost mode</span></span>

<span data-ttu-id="d04b5-109">Daha fazla bilgi için bkz: [Intune ile iOS/iPadOS aygıtlarında kayıp modu etkinleştir](https://docs.microsoft.com/intune/device-lost-mode) ve [Intune ile kaybolan veya çalınan iOS/iPadOS aygıtlarını bulun.](https://docs.microsoft.com/intune/device-locate)</span><span class="sxs-lookup"><span data-stu-id="d04b5-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="d04b5-110">**SSS**</span><span class="sxs-lookup"><span data-stu-id="d04b5-110">**FAQ**</span></span>

<span data-ttu-id="d04b5-111">S: Şirket verilerini bir aygıttan kaldırmak için uzaktan bir eylem yayınladım ve şimdi bekleyen bir durumda.</span><span class="sxs-lookup"><span data-stu-id="d04b5-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="d04b5-112">C: Uzaktan eylemin başarıyla tamamlanması için hedeflenen aygıtın çevrimiçi ve sağlıklı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d04b5-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="d04b5-113">Aşağıdaki durumlarda, uzak eylem 30 gün boyunca bekleme durumunda kalır veya aygıt komutu kabul edene kadar:</span><span class="sxs-lookup"><span data-stu-id="d04b5-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="d04b5-114">Aygıtın bağlantısı yoksa</span><span class="sxs-lookup"><span data-stu-id="d04b5-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="d04b5-115">Cihaz Intune ile yönetim durumunu kaybettiğinde</span><span class="sxs-lookup"><span data-stu-id="d04b5-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="d04b5-116">Bir aygıtın artık check-in olmadığını ve şirket verilerini kaldıramayacağını düşünüyorsanız Sil'i seçin.</span><span class="sxs-lookup"><span data-stu-id="d04b5-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="d04b5-117">Silme, aygıt kaydını kaldırarak aygıtların Intune listesinde artık görünmeyerek kaldırır.</span><span class="sxs-lookup"><span data-stu-id="d04b5-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="d04b5-118">Aygıt yeniden etkin hale gelirse, kullanıcısının yeniden kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="d04b5-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="d04b5-119">S: Neden bazı uzak eylemleri kullanmak için kullanılabilir değil mi?</span><span class="sxs-lookup"><span data-stu-id="d04b5-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="d04b5-120">C: Tüm platformlar tüm uzak aygıt eylemlerini desteklemez.</span><span class="sxs-lookup"><span data-stu-id="d04b5-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="d04b5-121">Aşağıdaki uzak eylemler platforma özgüdür, bu nedenle yalnızca belirtilen platformlar için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="d04b5-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="d04b5-122">Etkinleştirme Kilidini Atlama (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="d04b5-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="d04b5-123">Yeni Başlangıç (yalnızca Windows)</span><span class="sxs-lookup"><span data-stu-id="d04b5-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="d04b5-124">Kayıp modu (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="d04b5-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="d04b5-125">Aygıtı bulma (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="d04b5-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="d04b5-126">Yeniden başlat (yalnızca Windows)</span><span class="sxs-lookup"><span data-stu-id="d04b5-126">Restart (Windows only)</span></span>

<span data-ttu-id="d04b5-127">Her eylem hakkında daha fazla bilgi için [kullanılabilir aygıt eylemleri'ne](https://docs.microsoft.com/intune/device-management#available-device-actions)bakın.</span><span class="sxs-lookup"><span data-stu-id="d04b5-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>