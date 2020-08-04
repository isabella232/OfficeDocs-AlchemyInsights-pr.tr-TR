---
title: Son Nokta DLP'yi yapılandır
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556032"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="eb73d-102">Son Nokta DLP'yi yapılandır</span><span class="sxs-lookup"><span data-stu-id="eb73d-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="eb73d-103">Microsoft Endpoint DLP, DLP koruma ve izleme yeteneğini Windows 10 aygıtlarında hassas bilgilere genişletmenize olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="eb73d-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="eb73d-104">Aygıtlar aygıt yönetimine dahil edildikten sonra, öğeler üzerinde koruyucu eylemleri uygulamak için DLP ilkeleri oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eb73d-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="eb73d-105">Etkinlik Gezgini, hassas öğelerin etkinliğini izlemek için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="eb73d-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="eb73d-106">Daha fazla bilgi için, [aygıt yönetimine onboarding aygıtları](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)bakın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="eb73d-107">Endpoint DLP ile başlamak için:</span><span class="sxs-lookup"><span data-stu-id="eb73d-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="eb73d-108">Uygun SKU/abonelik lisanslama sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="eb73d-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="eb73d-109">Daha fazla bilgi için [SKU/abonelik lisanslama adresine](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)bakın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="eb73d-110">Cihaz yönetimini etkinleştirmek, biniş sayfasına erişmek veya cihaz izlemeyi açmak/kapatmak için gereken izinleri kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="eb73d-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="eb73d-111">Daha fazla bilgi için [İzinler'e](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)bakın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="eb73d-112">Onboard cihazları yordamını izleyerek Aygıt yönetimine dahil cihazlar.</span><span class="sxs-lookup"><span data-stu-id="eb73d-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="eb73d-113">M365 Uyumluluk **Ayarları**altındaki Device Onboarding (önizleme) seçeneğini kaçırıyorsanız, yukarıda belirtilen uygun lisans ve izinlere sahip olduğunuzu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="eb73d-114">Daha fazla bilgi için, [Onboarding aygıtları](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)bakın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="eb73d-115">Hassas öğelerinizi korumak için DLP ilkeleri oluşturun.</span><span class="sxs-lookup"><span data-stu-id="eb73d-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="eb73d-116">Daha fazla bilgi için [Endpoint DLP ilke senaryolarına](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)bakın.</span><span class="sxs-lookup"><span data-stu-id="eb73d-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="eb73d-117">Microsoft Endpoint DLP hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="eb73d-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>