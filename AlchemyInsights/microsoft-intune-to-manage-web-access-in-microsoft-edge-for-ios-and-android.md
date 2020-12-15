---
title: İOS ve Android için Microsoft Edge 'de Web erişimini yönetmek için Microsoft Intune kullanma
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679611"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="b56c9-102">İOS ve Android için Microsoft Edge 'de Web erişimini yönetmek için Microsoft Intune kullanma</span><span class="sxs-lookup"><span data-stu-id="b56c9-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="b56c9-103">İOS ve Android için Microsoft Edge, kullanıcının birden çok, tamamen ayrı profillerden Web 'de gözatmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="b56c9-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="b56c9-104">Microsoft Intune ve Azure Active Directory Premium özelliklerini içeren Enterprise Mobility + Güvenlik paketine (koşullu erişim gibi) abone olduğunuzda Microsoft 365 verilerinin en geniş koruma özellikleri kullanılabilir duruma gelir.</span><span class="sxs-lookup"><span data-stu-id="b56c9-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="b56c9-105">En azından, (1) bir koşullu erişim ilkesini dağıtmak isteyeceksiniz, kullanıcıların iOS ve Android için mobil cihazlardan Microsoft Edge 'e bağlanmasına olanak tanır ve bu (2), korumalı bir gözatma deneyimi sağlayan bir Microsoft Intune uygulaması koruma ilkesi uygular.</span><span class="sxs-lookup"><span data-stu-id="b56c9-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="b56c9-106">Koşullu erişim ve ilkeleri nasıl kullanabileceğinizi anlamak için bkz:</span><span class="sxs-lookup"><span data-stu-id="b56c9-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="b56c9-107">Azure Active Directory Koşullu erişim ilkelerini uygulama</span><span class="sxs-lookup"><span data-stu-id="b56c9-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="b56c9-108">Microsoft Intune uygulama koruma ilkeleri oluşturma</span><span class="sxs-lookup"><span data-stu-id="b56c9-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="b56c9-109">Azure Active Directory 'de çoklu oturum açmayı kullanma; ilke korumalı tarayıcılarda bağlı Web Apps</span><span class="sxs-lookup"><span data-stu-id="b56c9-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="b56c9-110">Gözatma deneyimini yönetmek için uygulama yapılandırmasını kullanma</span><span class="sxs-lookup"><span data-stu-id="b56c9-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="b56c9-111">Yalnızca iş ve okul hesaplarının kullanımına izin verme</span><span class="sxs-lookup"><span data-stu-id="b56c9-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="b56c9-112">Genel uygulama yapılandırma ilkelerini dağıtma</span><span class="sxs-lookup"><span data-stu-id="b56c9-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="b56c9-113">Veri koruma için uygulama yapılandırma ilkelerini dağıtma</span><span class="sxs-lookup"><span data-stu-id="b56c9-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="b56c9-114">Uygulama yapılandırma ilkelerini dağıtmak için Microsoft Endpoint Manager 'ı kullanma</span><span class="sxs-lookup"><span data-stu-id="b56c9-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="b56c9-115">Yönetilen uygulama günlüklerine erişmeyi öğrenmek için, [yönetilen uygulama günlüklerine erişmek üzere iOS ve Android Için Microsoft Edge kullanma](https://go.microsoft.com/fwlink/?linkid=2132578)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="b56c9-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
