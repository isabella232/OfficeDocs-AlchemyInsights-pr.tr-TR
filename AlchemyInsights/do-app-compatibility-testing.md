---
title: Uygulama uyumluluğu testi yapma
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
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694861"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="691d9-102">Uygulama uyumluluğu testi yapma</span><span class="sxs-lookup"><span data-stu-id="691d9-102">Do app compatibility testing</span></span>

<span data-ttu-id="691d9-103">Microsoft Edge için uygulama uyumluluğu son derece yüksektir.</span><span class="sxs-lookup"><span data-stu-id="691d9-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="691d9-104">Aslında, Microsoft'un aşağıdaki uyumluluk sözlerine sahip olması o kadar yüksektir:</span><span class="sxs-lookup"><span data-stu-id="691d9-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="691d9-105">Microsoft Edge 45 ve önceki sürümlerde çalışıyorsa, Microsoft Edge 77 ve sonraki sürümlerde çalışır.</span><span class="sxs-lookup"><span data-stu-id="691d9-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="691d9-106">Internet Explorer'da çalışıyorsa, Internet Explorer modunda Microsoft Edge'de çalışır.</span><span class="sxs-lookup"><span data-stu-id="691d9-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="691d9-107">Google Chrome'da çalışıyorsa Microsoft Edge'de çalışır.</span><span class="sxs-lookup"><span data-stu-id="691d9-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="691d9-108">Bu söze uymayacak bir uygulamanız varsa, Microsoft App Assure ile bunu düzeltme sözünün [arkasındayız.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="691d9-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="691d9-109">Bu söze rağmen, birçok kuruluşun bazı uygulamaları uyumluluk veya risk yönetimi nedenleriyle doğrulamaları gerektiğini biliyoruz.</span><span class="sxs-lookup"><span data-stu-id="691d9-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="691d9-110">Bunun çok açık olmasını beklese de, uygulama testlerinden düzenli ve sıkı bir şekilde organize olmak önemlidir.</span><span class="sxs-lookup"><span data-stu-id="691d9-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="691d9-111">Uygulama uyumluluk testinin iki yolu vardır:</span><span class="sxs-lookup"><span data-stu-id="691d9-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="691d9-112">**Laboratuvar testi:** Uygulamalar, belirli yapılandırmalarla sıkı denetimli bir ortamda test edilir.</span><span class="sxs-lookup"><span data-stu-id="691d9-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="691d9-113">**Pilot test:** Uygulamalar, kendi cihazlarını kullanarak günlük çalışma ortamında sınırlı sayıda kullanıcı tarafından test edilir.</span><span class="sxs-lookup"><span data-stu-id="691d9-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="691d9-114">Her uygulama için en uygun yöntemi seçin ve tüm kuruluşa başlatmadan önce testi kullanın.</span><span class="sxs-lookup"><span data-stu-id="691d9-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="691d9-115">Uygulamalarınızı uyumlu olduğundan emin olduktan sonra, Microsoft Edge'i bir pilot gruba dağıtmaya hazır oluruz.</span><span class="sxs-lookup"><span data-stu-id="691d9-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
