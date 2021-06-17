---
title: iOS Microsoft Intune Android için Microsoft Edge'de web erişimini yönetmek için Web Erişimini Kullanma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989726"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="18045-102">iOS Microsoft Intune Android için Microsoft Edge'de web erişimini yönetmek için Web Erişimini Kullanma</span><span class="sxs-lookup"><span data-stu-id="18045-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="18045-103">iOS Microsoft Edge Android uygulamaları, kullanıcının birden çok, tamamen ayrı profillerden web'de gezinmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="18045-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="18045-104">Microsoft 365 verileri için en geniş koruma özellikleri, koşullu erişim gibi Microsoft Intune ve Azure Active Directory Premium özellikleri içeren Enterprise Mobility + Security paketine abone olduğunda kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="18045-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="18045-105">En azından, (1) kullanıcıların mobil cihazlardan iOS ve Android için Microsoft Edge'e bağlanmalarına ve bu (2) korumalı göz atma deneyimi sağlayan bir Microsoft Intune uygulama koruma ilkesi uygulama ilkesi uygulamalarına olanak sağlayan bir koşullu erişim ilkesi dağıtmak istiyor olursunuz.</span><span class="sxs-lookup"><span data-stu-id="18045-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="18045-106">Koşullu erişimi ve ilkeleri nasıl kullanabileceğiniz hakkında bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="18045-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="18045-107">Koşullu Azure Active Directory ilkeleri uygulama</span><span class="sxs-lookup"><span data-stu-id="18045-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="18045-108">Uygulama Microsoft Intune ilkeleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="18045-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="18045-109">İlke korumalı tarayıcılarda bağlı Azure Active Directory web uygulamaları için çoklu oturum açma kullanma</span><span class="sxs-lookup"><span data-stu-id="18045-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="18045-110">Gözatma deneyimini yönetmek için uygulama yapılandırmasını kullanma</span><span class="sxs-lookup"><span data-stu-id="18045-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="18045-111">Yalnızca iş ve okul hesaplarının kullanımına izin verme</span><span class="sxs-lookup"><span data-stu-id="18045-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="18045-112">Genel uygulama yapılandırma ilkelerini dağıtma</span><span class="sxs-lookup"><span data-stu-id="18045-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="18045-113">Veri koruması için uygulama yapılandırma ilkelerini dağıtma</span><span class="sxs-lookup"><span data-stu-id="18045-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="18045-114">Uygulama Microsoft Endpoint Manager ilkelerini dağıtmak için kullanıcı ayarlarını kullanma</span><span class="sxs-lookup"><span data-stu-id="18045-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="18045-115">Yönetilen uygulama günlüklerine nasıl erişil olduğunu öğrenmek için bkz. Yönetilen uygulama [günlüklerine erişmek Microsoft Edge iOS ve Android için Microsoft Edge](https://go.microsoft.com/fwlink/?linkid=2132578)kullanma .</span><span class="sxs-lookup"><span data-stu-id="18045-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
