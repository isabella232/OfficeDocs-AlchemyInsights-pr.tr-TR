---
title: Intune ile özel bildirimler gönderme
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720666"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="fe59f-102">Yönetilen iOS ve Android aygıtlarının kullanıcılarına özel bildirimler gönderme</span><span class="sxs-lookup"><span data-stu-id="fe59f-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="fe59f-103">Intune için özel bildirimler, kullanıcının aygıtındaki Şirket portalı uygulaması tarafından işlenir.</span><span class="sxs-lookup"><span data-stu-id="fe59f-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="fe59f-104">Uygulama o cihazda anında bildirim oluşturur.</span><span class="sxs-lookup"><span data-stu-id="fe59f-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="fe59f-105">Aşağıda, özel bildirimlerin alındığını destekleyen cihaz önkoşulları ve uygulama için anında bildirim oluşturulması sağlanır:</span><span class="sxs-lookup"><span data-stu-id="fe59f-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="fe59f-106">Cihazda Şirket portalı uygulaması yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fe59f-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="fe59f-107">Cihazın, Şirket portalı uygulamasının anında bildirim göndermesine izin vermesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="fe59f-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="fe59f-108">Uygulama yüklendiğinde veya güncelleştirildiğinde kullanıcıya bildirimlere izin vermesi istenir.</span><span class="sxs-lookup"><span data-stu-id="fe59f-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="fe59f-109">Android cihazlarda Google Play Hizmetleri yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fe59f-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="fe59f-110">Cihaz Intune 'a kaydolmalıdır.</span><span class="sxs-lookup"><span data-stu-id="fe59f-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="fe59f-111">İleti gönderme hakkında daha fazla bilgi için [özellik belgelerine](https://docs.microsoft.com/intune/custom-notifications)bakın.</span><span class="sxs-lookup"><span data-stu-id="fe59f-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
