---
title: Intune ile özel bildirimler gönderme
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886877"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="01f7b-102">Yönetilen iOS ve Android cihazların kullanıcılarına özel bildirimler nasıl gönderilir?</span><span class="sxs-lookup"><span data-stu-id="01f7b-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="01f7b-103">Intune için özel bildirimler, Şirket Portalı uygulaması tarafından kullanıcının cihazında işlenir.</span><span class="sxs-lookup"><span data-stu-id="01f7b-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="01f7b-104">Uygulama daha sonra bu cihazda anında iletme bildirimi oluşturur.</span><span class="sxs-lookup"><span data-stu-id="01f7b-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="01f7b-105">Özel bildirimlerin alınmasını desteklemek ve uygulamanın daha sonra anında iletme bildirimini oluşturması için cihaz ön koşulları şunlardır:</span><span class="sxs-lookup"><span data-stu-id="01f7b-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="01f7b-106">Cihaz, Şirket Portalı uygulamasını yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="01f7b-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="01f7b-107">Cihaz, Şirket Portalı uygulamasının anında iletme bildirimleri göndermesine izin vermelidir.</span><span class="sxs-lookup"><span data-stu-id="01f7b-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="01f7b-108">Uygulama yüklendiğinde veya güncelleştirildiğinde, kullanıcıdan bildirimlere izin vermesini ister.</span><span class="sxs-lookup"><span data-stu-id="01f7b-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="01f7b-109">Android cihazlarda Google Play Hizmetleri yüklü olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="01f7b-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="01f7b-110">Cihaz Intune ile kayıtlı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="01f7b-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="01f7b-111">İleti nin nasıl gönderilebildiğini de içeren daha fazla bilgi için [özellik belgelerine](https://docs.microsoft.com/intune/custom-notifications)bakın.</span><span class="sxs-lookup"><span data-stu-id="01f7b-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
