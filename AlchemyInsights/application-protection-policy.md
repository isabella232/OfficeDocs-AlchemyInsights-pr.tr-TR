---
title: Uygulama koruma ilkesi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423957"
---
# <a name="application-protection-policy"></a><span data-ttu-id="de411-102">Uygulama koruma ilkesi</span><span class="sxs-lookup"><span data-stu-id="de411-102">Application protection policy</span></span>

<span data-ttu-id="de411-103">Uygulama koruma politikasında (APP) yeniyseniz, [Uygulama koruma politikalarına genel bakışa](https://docs.microsoft.com/intune/apps/app-protection-policy)göz atın.</span><span class="sxs-lookup"><span data-stu-id="de411-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="de411-104">APP'i kullanmaya başlamak [için, uygulama koruma ilkelerini nasıl oluşturup atayabilirsiniz'a](https://docs.microsoft.com/intune/app-protection-policies)bakın.</span><span class="sxs-lookup"><span data-stu-id="de411-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="de411-105">Uygulama koruma ilkesi gereksinimleri:</span><span class="sxs-lookup"><span data-stu-id="de411-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="de411-106">Kullanıcının Intune veya EMS lisansı vardır.</span><span class="sxs-lookup"><span data-stu-id="de411-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="de411-107">Kullanıcı, uygulama koruma ilkeleri tarafından hedeflenen bir gruba aittir.</span><span class="sxs-lookup"><span data-stu-id="de411-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="de411-108">Aygıttaki korumalı uygulamalarda yalnızca bir şirket kullanıcısı oturum açmış.</span><span class="sxs-lookup"><span data-stu-id="de411-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="de411-109">Uygulama [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)uygulanmıştır.</span><span class="sxs-lookup"><span data-stu-id="de411-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="de411-110">SDK'yı destekleyen uygulamaların listesi için [Microsoft Intune korumalı uygulamalara](https://docs.microsoft.com/intune/apps-supported-intune-apps)bakın.</span><span class="sxs-lookup"><span data-stu-id="de411-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="de411-111">İlkeler, yukarıdaki gereksinimleri karşılayan bir kullanıcı intune SDK etkin bir uygulamaya işaret ettikten sonra uygulanır.</span><span class="sxs-lookup"><span data-stu-id="de411-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="de411-112">Bir ilkenin uygulanıp uygulanmadığını belirlemenin en kolay yolu, kullanıcının ilkede bir pin ayarlamasını gerektirmektir.</span><span class="sxs-lookup"><span data-stu-id="de411-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="de411-113">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="de411-113">For more information, see:</span></span>

[<span data-ttu-id="de411-114">APP/MAM sorun giderme SSS</span><span class="sxs-lookup"><span data-stu-id="de411-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="de411-115">Uygulama koruma ilkesi kurulumunuzu doğrulama</span><span class="sxs-lookup"><span data-stu-id="de411-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="de411-116">Uygulama Koruma Politikası'nın teslim zamanlamasını anlayın</span><span class="sxs-lookup"><span data-stu-id="de411-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="de411-117">Uygulama koruma ilkeleri nasıl izlenir?</span><span class="sxs-lookup"><span data-stu-id="de411-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)