---
title: Var olan tarayıcı ortamınızı değerlendirme ve hedefleri tanımlama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694818"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="f7f4c-102">Var olan tarayıcı ortamınızı değerlendirme ve hedefleri tanımlama</span><span class="sxs-lookup"><span data-stu-id="f7f4c-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="f7f4c-103">Geçerli tarayıcının durumunu ve proje görüşünü anlamak için zaman almak, tüm proje katılımcılarının uyumlu ve aynı hedefe yönelik çalışmalarına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="f7f4c-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="f7f4c-104">Şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="f7f4c-104">Follow these steps:</span></span>

1. <span data-ttu-id="f7f4c-105">Geçerli eyaletinizi tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="f7f4c-105">Define your current state.</span></span> <span data-ttu-id="f7f4c-106">Şunları göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="f7f4c-106">Consider the following:</span></span>
- <span data-ttu-id="f7f4c-107">Şu anda ortamınıza hangi tarayıcılar dağıtılır?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="f7f4c-108">Hangi tarayıcı varsayılan tarayıcı olarak ayarlanır?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="f7f4c-109">Uygulamalarınızı bazıları için Internet Explorer'ı kullanmak zorunda mısınız?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="f7f4c-110">Internet Explorer'ı bugün yapılandırmak için Kurumsal Mod Site Listesi mi kullanıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="f7f4c-111">Ortamınız Windows 10 ve macOS gibi hangi işletim sistemi platformlarını destekliyor?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="f7f4c-112">Tarayıcı yönetimi için hangi yönetim araçlarını kullanırsınız?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="f7f4c-113">Tarayıcı yapılandırması ve yönetiminden sorumlu olan kimdir?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="f7f4c-114">Tarayıcı uyumluluğunu doğrulama işlemi nedir?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="f7f4c-115">Dağıtımınız için hedefleri tanımlayın.</span><span class="sxs-lookup"><span data-stu-id="f7f4c-115">Define the goals for your deployment.</span></span> <span data-ttu-id="f7f4c-116">Aşağıdaki şeyleri unutmayın:</span><span class="sxs-lookup"><span data-stu-id="f7f4c-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="f7f4c-117">[Microsoft Edge'i varsayılan tarayıcınız olarak ayarlamak istiyor musunuz?](https://docs.microsoft.com/DeployEdge/edge-default-browser)</span><span class="sxs-lookup"><span data-stu-id="f7f4c-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="f7f4c-118">Microsoft Edge'in eski sürümünü gizlemek mi yoksa kullanıcıların kullanımına açık bırakmak [mı istiyorsunuz?](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)</span><span class="sxs-lookup"><span data-stu-id="f7f4c-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="f7f4c-119">[Microsoft Edge'i nasıl yapılandıracaksınız?](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)</span><span class="sxs-lookup"><span data-stu-id="f7f4c-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="f7f4c-120">İlk dağıtımınız kapsamında yapılandırmak için hangi özellikler kritik öneme sahiptir?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="f7f4c-121">Tanımlanan herhangi bir uyumluluk veya yapılandırma sorununa yönelik işlem nedir?</span><span class="sxs-lookup"><span data-stu-id="f7f4c-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="f7f4c-122">Kullanmak istediğiniz özelliklerin önkoşullarını anlıyoruz, örneğin:</span><span class="sxs-lookup"><span data-stu-id="f7f4c-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="f7f4c-123">Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="f7f4c-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="f7f4c-124">Internet Explorer modu</span><span class="sxs-lookup"><span data-stu-id="f7f4c-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="f7f4c-125">Kimlik doğrulama ve eşitleme</span><span class="sxs-lookup"><span data-stu-id="f7f4c-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="f7f4c-126">Bu adımları tamamlandıktan sonra, dağıtım stratejinizi planlamaya başlamaya hazır oluruz.</span><span class="sxs-lookup"><span data-stu-id="f7f4c-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
