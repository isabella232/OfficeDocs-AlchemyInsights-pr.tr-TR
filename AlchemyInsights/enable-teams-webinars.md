---
title: Web seminerlerini Teams etkinleştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794036"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="bad70-102">Web seminerlerini Teams etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="bad70-102">Enable Teams Webinars</span></span>

<span data-ttu-id="bad70-103">Web seminerleri varsayılan olarak etkindir.</span><span class="sxs-lookup"><span data-stu-id="bad70-103">Webinars are enabled by default.</span></span> <span data-ttu-id="bad70-104">Teams PowerShell komutlarını kullanarak, Web seminerleri için kimlerin zaman Teams kaydola bir şekilde yönetebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="bad70-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="bad70-105">Toplantı oluşturan tüm kullanıcılar, web amaçlı toplantı da oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="bad70-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="bad70-106">Web seminerleri için kimlerin zaman Teams yönetmek için *AllowMeetingRegistration kullanın.*</span><span class="sxs-lookup"><span data-stu-id="bad70-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="bad70-107">Varsayılan olarak, *WhoCanRegister* etkindir ve Herkes olarak **ayarlanır.**</span><span class="sxs-lookup"><span data-stu-id="bad70-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="bad70-108">Toplantı kaydını kapatmak için *AllowMeetingRegistration'i* False olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="bad70-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="bad70-109">Bu ayarları değiştirmek için, Teams [PowerShell yüklemeniz gerekir.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="bad70-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="bad70-110">Ayrıca, Toplantı İlkeleri web seminerleri Teams uygulanır.</span><span class="sxs-lookup"><span data-stu-id="bad70-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="bad70-111">Örneğin, toplantı ayarlarında anonim katılma kapalı ise, anonim kullanıcılar web seminerine kat değildir.</span><span class="sxs-lookup"><span data-stu-id="bad70-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="bad70-112">Web seminerleri için kimlerin kaydol etkiyiyi yapılandırma hakkında daha fazla bilgi edinmek için bkz. [Web seminerleri için kimlerin kaydol etkiyi yapılandır?](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="bad70-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="bad70-113">Microsoft Listeleri ayarları hakkında daha fazla bilgi için bkz. [Microsoft Listeleri için ayarları denetleme.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="bad70-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>