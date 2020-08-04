---
title: Intune'da bayat cihazların otomatik olarak temizlenmesi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555737"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="5092a-102">Intune'da bayat cihazların otomatik olarak temizlenmesi</span><span class="sxs-lookup"><span data-stu-id="5092a-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="5092a-103">Intune, yöneticinin 90 ile 270 gün arasında bir zaman aralığı yapılandırmasına olanak tanır ve bu süre den sonra eski aygıtlar hizmetten kaldırılır.</span><span class="sxs-lookup"><span data-stu-id="5092a-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="5092a-104">Bu ayar kuruluş genelindedir ve etkinleştirildiğinde hemen yürürlüğe girer.</span><span class="sxs-lookup"><span data-stu-id="5092a-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="5092a-105">Ayarı aşan bir süre için Intune sunucusunda denetlenen tüm aygıtlar kalıcı olarak silinir.</span><span class="sxs-lookup"><span data-stu-id="5092a-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="5092a-106">**Not** Bu temizleme eylemi için yalnızca MDM aygıt nesneleri uygundur.</span><span class="sxs-lookup"><span data-stu-id="5092a-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="5092a-107">EAS yalnızca aygıt nesneleri hariç tutulur.</span><span class="sxs-lookup"><span data-stu-id="5092a-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="5092a-108">Bir aygıtın aygıt temizleme kurulumuna ve "durumuna" bağlı olarak silinme için ne zaman uygun hale gelmesi hakkında daha fazla bilgi için:</span><span class="sxs-lookup"><span data-stu-id="5092a-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="5092a-109">Ayar: **Son iade tarihinden sonra aygıtları silme: Evet (belirtilen günlerde bazı değer (N))**</span><span class="sxs-lookup"><span data-stu-id="5092a-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="5092a-110">Ayarda yapılandırılan değer (N) değerine göre, Intune hizmeti aygıtı son başarıyla giriş yaptıktan sonraki gün içinde siler.</span><span class="sxs-lookup"><span data-stu-id="5092a-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="5092a-111">Ayar: **Son iade tarihinden sonra aygıtları silme: Hayır**</span><span class="sxs-lookup"><span data-stu-id="5092a-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="5092a-112">Cihaz sertifikasının süresi dolduktan ve yenilenmedikten 180 gün sonra aygıt silinir.</span><span class="sxs-lookup"><span data-stu-id="5092a-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="5092a-113">**Not** Her iki durumda da, aygıtın Intune'da başarıyla kaydedilmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="5092a-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="5092a-114">Kayıt, Intune hizmetiyle yapılan ilk cihaz denetimi sırasında gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="5092a-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="5092a-115">Bir aygıt Başarılı bir şekilde Intune'a kaydolursa ancak Intune kayıtlı değilse, aygıt kayıttan 270 gün sonra silinir.</span><span class="sxs-lookup"><span data-stu-id="5092a-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="5092a-116">(Aygıtı iptal edilmiş olarak işaretlemek için 90 gün, kaydı silmek için ise 180 gün daha.)</span><span class="sxs-lookup"><span data-stu-id="5092a-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="5092a-117">Şu anda Intune konsolunda, belirli bir aygıt için aygıt sertifikasının son kullanma tarihini belirlemek için bir mekanizma bulunmamaktadır.</span><span class="sxs-lookup"><span data-stu-id="5092a-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>