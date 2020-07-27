---
title: Intune ile denetlenen iOS aygıtlarında etkinleştirme kilidini atlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424209"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="3b2a2-102">Intune ile denetlenen iOS aygıtlarında etkinleştirme kilidini atlama</span><span class="sxs-lookup"><span data-stu-id="3b2a2-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="3b2a2-103">iOS aygıtlarında etkinleştirme kilidini atlayabilmesi, kullanıcının bir şirket aygıtında etkinleştirme kilidini etkinleştirdiği ve ardından şirketten ayrıldığı senaryodan kurtulmayı kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="3b2a2-104">Etkinleştirme kilidini atlamak için ön koşullar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="3b2a2-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="3b2a2-105">"Denetlenen" bir aygıttır.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="3b2a2-106">Etkinleştirme kilidi, Intune'da iOS Aygıt kısıtlama ilkesi kullanılarak başarıyla etkinleştirilir.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="3b2a2-107">Ayrıca, etkinleştirme kilidini atlarken şunları</span><span class="sxs-lookup"><span data-stu-id="3b2a2-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="3b2a2-108">Fiziksel olarak silinen cihaza sahip.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="3b2a2-109">Silmeyi vermeden önce kodu kopyalayın.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="3b2a2-110">**Not:** Silme kodu büyük/küçük harf duyarlı değildir, bu nedenle "-" karakterler gerekli değildir.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="3b2a2-111">Ayrıntılar için, [Intune'a sahip Denetlenen iOS aygıtlarında Etkinleştirme Kilidini Bypass'a](https://docs.microsoft.com/intune/device-activation-lock-bypass)bakın.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="3b2a2-112">**SSS**</span><span class="sxs-lookup"><span data-stu-id="3b2a2-112">**FAQ**</span></span>

<span data-ttu-id="3b2a2-113">S: **Şirket verilerini bir aygıttan kaldırmak için uzaktan bir eylem yayınladım ve şimdi bekleyen bir durumda.**</span><span class="sxs-lookup"><span data-stu-id="3b2a2-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="3b2a2-114">C: Uzaktan eylemin başarıyla tamamlanması için hedeflenen aygıtın çevrimiçi ve sağlıklı olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="3b2a2-115">Aşağıdaki durumlarda, uzak eylem 30 gün boyunca bekleme durumunda kalır veya aygıt aşağıdaki durumlarda komutu kabul edene kadar:</span><span class="sxs-lookup"><span data-stu-id="3b2a2-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="3b2a2-116">Bağlantı yok.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-116">Does not have connectivity.</span></span>
- <span data-ttu-id="3b2a2-117">Intune ile yönetim statüsünü kaybeder.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="3b2a2-118">Aygıtın artık check-in olmadığını ve şirket verilerini kaldırmayacağını düşünüyorsanız Sil'i seçin.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="3b2a2-119">Silme, aygıt kaydını kaldırarak aygıtların Intune listesinde artık görünmeyerek kaldırır.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="3b2a2-120">Aygıtın yeniden etkin hale gelmesi için, kullanıcının aygıtı yeniden kaydetmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="3b2a2-121">S: **Neden bazı uzak eylemleri kullanmak için kullanılabilir değil mi?**</span><span class="sxs-lookup"><span data-stu-id="3b2a2-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="3b2a2-122">C: Tüm platformlar tüm uzak aygıt eylemlerini desteklemez.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="3b2a2-123">Aşağıdaki uzak eylemler platforma özgüdür.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="3b2a2-124">Etkinleştirme Kilidini Atlama (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="3b2a2-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="3b2a2-125">Yeni Başlangıç (yalnızca Windows)</span><span class="sxs-lookup"><span data-stu-id="3b2a2-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="3b2a2-126">Kayıp modu (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="3b2a2-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="3b2a2-127">Aygıtı bulma (yalnızca iOS)</span><span class="sxs-lookup"><span data-stu-id="3b2a2-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="3b2a2-128">Yeniden başlat (yalnızca Windows)</span><span class="sxs-lookup"><span data-stu-id="3b2a2-128">Restart (Windows only)</span></span>

<span data-ttu-id="3b2a2-129">Her eylem hakkında daha fazla bilgi için [kullanılabilir aygıt eylemleri'ne](https://docs.microsoft.com/intune/device-management#available-device-actions)bakın.</span><span class="sxs-lookup"><span data-stu-id="3b2a2-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>