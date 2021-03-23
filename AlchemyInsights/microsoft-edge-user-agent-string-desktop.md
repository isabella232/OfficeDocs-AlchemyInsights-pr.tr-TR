---
title: Microsoft Edge kullanıcı aracısı dizeleri (Masaüstü)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8221"
- "9004596"
ms.openlocfilehash: 42c39f5661f57c7b57fa471f9c204e5c27f2f214
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037299"
---
# <a name="microsoft-edge-user-agent-strings-desktop"></a><span data-ttu-id="84fa7-102">Microsoft Edge kullanıcı aracısı dizeleri (Masaüstü)</span><span class="sxs-lookup"><span data-stu-id="84fa7-102">Microsoft Edge user agent strings (Desktop)</span></span>

<span data-ttu-id="84fa7-103">Kullanıcı aracısı (UA) dizeleri belirli bir işletim sisteminde belirli bir tarayıcının hangi sürümünün kullanılıyor olduğunu saptamak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="84fa7-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="84fa7-104">Diğer tarayıcılarda olduğu gibi, Microsoft Edge de siteye her istekte bulunan "Kullanıcı-Aracısı" HTTP üst bilgisinde bu bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="84fa7-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="84fa7-105">Ayrıca, JavaScript aracılığıyla "navigator.userAgent" değerini sorgu yoluyla da erişilebilir.</span><span class="sxs-lookup"><span data-stu-id="84fa7-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="84fa7-106">Web geliştiricilerinin, kod bakımını geliştirmek, kod dayanıklılığını azaltmak ve gelecek UA dizesi güncelleştirmeleri durumunda kod kesintisi riskini ortadan kaldırmak için mümkün olduğunca özellik algılamayı kullanmalarını öneririz.</span><span class="sxs-lookup"><span data-stu-id="84fa7-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="84fa7-107">Daha fazla bilgi için [bkz. Microsoft Edge Kullanıcı Aracısı Dizesi (Masaüstü).](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)</span><span class="sxs-lookup"><span data-stu-id="84fa7-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>

