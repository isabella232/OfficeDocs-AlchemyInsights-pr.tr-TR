---
title: Defender Endpoint check sensor status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676543"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="b160f-102">Defender Endpoint check sensor status</span><span class="sxs-lookup"><span data-stu-id="b160f-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="b160f-103">Algılayıcı **sorunu olan cihazlar kutucuğu** Güvenlik İşlemleri panosunda bulunur.</span><span class="sxs-lookup"><span data-stu-id="b160f-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="b160f-104">Bu kutucuk, ayrı ayrı cihazın algılayıcı verilerini sağlayabilme ve Uç Nokta için Defender hizmetiyle iletişim kurma özelliği hakkında bilgi sağlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="b160f-105">Bu rapor, kaç cihazla dikkat gerektir olduğunu rapor etmektedir ve sorunlu cihazları tanımları ve bilinen sorunları düzeltmeye yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="b160f-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="b160f-106">Kutucukta yer alan iki durum göstergesi, hizmete düzgün bir şekilde rapornabilecek cihaz sayısı hakkında bilgi sağlar:</span><span class="sxs-lookup"><span data-stu-id="b160f-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="b160f-107">**Hatalı Yapılandırılmış** Kısmen algılayıcı verilerini Uç Nokta için Defender hizmetine bildiren ve düzeltilmesi gereken yapılandırma hataları olan cihazlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="b160f-108">**Etkin değil** Geçen ay yediden fazla gün boyunca Uç Nokta için Defender hizmetine bildirmeyi durduran cihazlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="b160f-109">Gruplardan herhangi birini tıklatmak sizi seçeneklere göre filtrelenmiş olarak Cihazlar listesine yönlendirmektedir.</span><span class="sxs-lookup"><span data-stu-id="b160f-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="b160f-110">Cihazlar listesinde durum listesini aşağıdaki durum durumuna göre filtre yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b160f-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="b160f-111">**Etkin** Etkin olarak Uç nokta için Defender hizmetine rapor yapan cihazlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="b160f-112">**Hatalı Yapılandırılmış** Kısmen algılayıcı verilerini Uç Nokta için Defender hizmetine bildiriyor ama düzeltilmesi gereken yapılandırma hataları olan cihazlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="b160f-113">Yanlış yapılandırılmış cihazlar aşağıdaki sorunlardan birini veya bir birleşimine sahip olabilir:</span><span class="sxs-lookup"><span data-stu-id="b160f-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="b160f-114">Algılayıcı verisi yok - Cihazlar algılayıcı verilerini göndermeyi durdurdu.</span><span class="sxs-lookup"><span data-stu-id="b160f-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="b160f-115">Cihazdan sınırlı uyarılar tetiklenir.</span><span class="sxs-lookup"><span data-stu-id="b160f-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="b160f-116">İletişim engelli - Cihazla iletişim kurma yeteneği engellidir.</span><span class="sxs-lookup"><span data-stu-id="b160f-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="b160f-117">Daha derin çözümleme yapmak, dosyaları engellemek, cihazı ağdan ve cihazla iletişim gerektiren diğer eylemlerden göndermek işe yaramadı.</span><span class="sxs-lookup"><span data-stu-id="b160f-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="b160f-118">**Etkin değil** Uç nokta için Defender hizmetine bildirmeyi durduran cihazlar.</span><span class="sxs-lookup"><span data-stu-id="b160f-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="b160f-119">Dışarı Aktar özelliğini kullanarak listenin tamamını CSV biçiminde indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b160f-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="b160f-120">Daha fazla bilgi için [bkz. Uç Nokta için Microsoft Defender'da algılayıcıların durumunu denetleme.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="b160f-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="b160f-121">Bir cihazın devre dışı veya hatalı yapılandırılmasına neyin neden olduğu hakkında daha fazla bilgi için bkz. Uç Nokta için Microsoft Defender'daki uygun olmayan [algılayıcıları düzeltme](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="b160f-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
