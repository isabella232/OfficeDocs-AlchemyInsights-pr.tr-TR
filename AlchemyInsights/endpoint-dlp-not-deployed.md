---
title: Kullanıcının cihazına dağıtıldıktan sonra uç nokta DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731871"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="8a6dd-102">Kullanıcının cihazına dağıtıldıktan sonra uç nokta DLP</span><span class="sxs-lookup"><span data-stu-id="8a6dd-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="8a6dd-103">Kullanıcının cihazına Uç nokta veri kaybı önleme (DLP) ayarı uygulanmadı ise, şu gereksinimleri karşıla uygulandığını onaylayın:</span><span class="sxs-lookup"><span data-stu-id="8a6dd-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="8a6dd-104">Windows 10 x64 derleme 1809 veya sonraki bir sürümü cihaza yüklenir.</span><span class="sxs-lookup"><span data-stu-id="8a6dd-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="8a6dd-105">Kötü amaçlı yazılımdan koruma istemci sürümü 4.18.2009.7 veya sonrası yüklenir.</span><span class="sxs-lookup"><span data-stu-id="8a6dd-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="8a6dd-106">Cihaz şu **kişilerden** biridir:</span><span class="sxs-lookup"><span data-stu-id="8a6dd-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="8a6dd-107">Azure Active Directory (Azure AD) katıldı</span><span class="sxs-lookup"><span data-stu-id="8a6dd-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="8a6dd-108">Karma Azure AD'ye katıldı</span><span class="sxs-lookup"><span data-stu-id="8a6dd-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="8a6dd-109">AAD kaydedildi</span><span class="sxs-lookup"><span data-stu-id="8a6dd-109">AAD registered</span></span>

- <span data-ttu-id="8a6dd-110">İlke eylemlerini zorunlu yapmak için, Microsoft Chromium uç nokta cihazına Microsoft Edge tarayıcısının yüklü olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="8a6dd-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="8a6dd-111">Uç Nokta DLP'nin dağıtımına yönelik ek gereksinimler için [bkz. Uç nokta veri kaybı önleme ile çalışmaya başlama.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="8a6dd-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>