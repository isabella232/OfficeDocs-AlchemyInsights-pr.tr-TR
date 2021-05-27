---
title: Yazılım stoku eksik veya yanlış
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676588"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="7cb6d-102">Yazılım stoku eksik veya yanlış</span><span class="sxs-lookup"><span data-stu-id="7cb6d-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="7cb6d-103">TVM)'Tehdit ve Güvenlik Açığı Yönetimi yazılım envanteri, resmi Ortak Platform Enumerations (CPE) ile, kuruluşta bilinen yazılımların bir listesidir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="7cb6d-104">Resmi CPE olmayan yazılım ürünleri, yayımlanmış güvenlik açıklarına sahip değildir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="7cb6d-105">Stokta ayrıca satıcının adı, zayıf noktaların sayısı, tehdit ve açık cihaz sayısı gibi ayrıntılar da yer amektedir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="7cb6d-106">Cihazlardaki yazılım değişiklikleri genellikle iki saat içinde güvenlik portallarına yansır.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="7cb6d-107">Bununla birlikte, bazen daha uzun sürebilir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="7cb6d-108">Şu anda eşitlemeyi zorlamanın bir yolu yoktur; bu sürekli bir sürekli değerlendirmedir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="7cb6d-109">Bir yazılım değişikliği yaptınız ve bu değişiklik 5 saat sonra TVM'ye doğru şekilde yansıtıldısa şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="7cb6d-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="7cb6d-110">Yazılımın nasıl algılandığından anlamak için yazılım kanıtı bölümünü kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="7cb6d-111">Yazılımın destek olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-111">Make sure that the software is supported.</span></span> <span data-ttu-id="7cb6d-112">Yazılım, şu anda yazılım destekçisi tarafından desteklenemeyebilir ve cihaz Tehdit ve Güvenlik Açığı Yönetimi.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="7cb6d-113">Bununla birlikte, yalnızca sınırlı veriler kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="7cb6d-114">Portaldan yanlışlığı bildirme adımları için bkz. [Hatalı raporu bildirme](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="7cb6d-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="7cb6d-115">**Not:** MDE portalında bir yanlışlığı raporlamak mühendislik için tek yollu bir kanaldır.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="7cb6d-116">Sorun acilse bir destek bileti açın.</span><span class="sxs-lookup"><span data-stu-id="7cb6d-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="7cb6d-117">Daha fazla bilgi için [bkz. Yazılım envanteri - Tehdit ve Güvenlik Açığı Yönetimi.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="7cb6d-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>