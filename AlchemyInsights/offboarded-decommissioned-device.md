---
title: Cihaz Envanteri'ne çıkarma veya çıkarma cihazı kaldırmayla ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564612"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="82e8c-102">Cihaz Envanteri'ne çıkarma veya çıkarma cihazı kaldırmayla ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="82e8c-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="82e8c-103">Uç Nokta için Microsoft Defender şu anda çıkarma veya çıkarma cihazın cihaz kaydının Cihaz Envanteri'nden el ile kaldırılmasına izin vermiyor.</span><span class="sxs-lookup"><span data-stu-id="82e8c-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="82e8c-104">Güvenlik nedeniyle, cihaz portalda 180 gün boyunca geçmiş bir kayıt olarak kalır.</span><span class="sxs-lookup"><span data-stu-id="82e8c-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="82e8c-105">Bununla birlikte, cihaz verileri yapılandırılmış bekletme sürenize göre temiz olur.</span><span class="sxs-lookup"><span data-stu-id="82e8c-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="82e8c-106">**Not:** Çıkarılırken veya çıkarılırken cihaz yedi gün sonra otomatik olarak **Etkin Değil** durumuna gelir.</span><span class="sxs-lookup"><span data-stu-id="82e8c-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="82e8c-107">Buna ek olarak, son 30 gün içinde etkin durumdaki cihazlar, organizasyon puanınızı veya Cihazlar için Microsoft Güvenli Puanı'Tehdit ve Güvenlik Açığı Yönetimi olan verilere faktör değildir.</span><span class="sxs-lookup"><span data-stu-id="82e8c-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="82e8c-108">Cihaz Envanteri görünümünde bazı cihazları yine de görmek istemiyorsanız, kaldırilen cihazı Cihaz Envanteri görünümünden filtrelemek için bir cihaz etiketi yerleştirmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="82e8c-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="82e8c-109">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="82e8c-109">For more information, see:</span></span>

[<span data-ttu-id="82e8c-110">Uç nokta için Microsoft Defender hizmetinin offboard cihazları</span><span class="sxs-lookup"><span data-stu-id="82e8c-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="82e8c-111">Sayılarda pozlama Tehdit ve Güvenlik Açığı Yönetimi</span><span class="sxs-lookup"><span data-stu-id="82e8c-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="82e8c-112">Uç Nokta için Microsoft Defender'da uygun olmayan algılayıcıları düzeltme</span><span class="sxs-lookup"><span data-stu-id="82e8c-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="82e8c-113">Etiketlemeyi etkili bir şekilde kullanma (Bölüm 1)</span><span class="sxs-lookup"><span data-stu-id="82e8c-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="82e8c-114">Etiketlemeyi etkili bir şekilde kullanma (Bölüm 2)</span><span class="sxs-lookup"><span data-stu-id="82e8c-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="82e8c-115">Etiketlemeyi etkili bir şekilde kullanma (Bölüm 3)</span><span class="sxs-lookup"><span data-stu-id="82e8c-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




