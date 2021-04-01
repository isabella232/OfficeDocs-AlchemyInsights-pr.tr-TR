---
title: MacOS cihazında Microsoft Edge'i varsayılan tarayıcı olarak ayarlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491818"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="6c310-102">MacOS cihazında Microsoft Edge'i varsayılan tarayıcı olarak ayarlama</span><span class="sxs-lookup"><span data-stu-id="6c310-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="6c310-103">Microsoft Edge'i varsayılan tarayıcı olarak ayarlamak için şu iki yöntemden birini kullanın:</span><span class="sxs-lookup"><span data-stu-id="6c310-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="6c310-104">Yöntem 1: Microsoft Edge'in zaten varsayılan tarayıcı olarak ayarlanmış olduğu bir macOS resmiyle cihazı flaş gibi yanıp söner.</span><span class="sxs-lookup"><span data-stu-id="6c310-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="6c310-105">Yöntem 2: Kullanıcıdan Microsoft Edge'i varsayılan tarayıcı olarak ayarlamasını istenirken DefaultBrowserSettingEnabled ilkesi ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="6c310-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="6c310-106">Her iki yöntem de kullanıcının varsayılan tarayıcıyı değiştirmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="6c310-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="6c310-107">Bu nedenle, 1. yöntemi kullansanız bile DefaultBrowserSettingEnabled ilkesini dağıtmanız önerilir.</span><span class="sxs-lookup"><span data-stu-id="6c310-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="6c310-108">İlke dağıtıldıktan sonra kullanıcı varsayılan tarayıcıyı değiştirirse, ilke kullanıcıdan varsayılan tarayıcıyı Microsoft Edge'e geri ayarlamasını istenir.</span><span class="sxs-lookup"><span data-stu-id="6c310-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
