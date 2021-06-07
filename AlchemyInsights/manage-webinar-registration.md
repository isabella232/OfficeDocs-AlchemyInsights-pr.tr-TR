---
title: Web ziyareti kaydını yönetme
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794143"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2ba2b-102">Web ziyareti kaydını yönetme</span><span class="sxs-lookup"><span data-stu-id="2ba2b-102">Manage webinar registration</span></span>

<span data-ttu-id="2ba2b-103">Web seminerleri için kimlerin Teams Powershell komutlarını Teams yönetirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2ba2b-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="2ba2b-104">Powershell'Teams yüklemek için bkz. [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="2ba2b-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="2ba2b-105">Varsayılan olarak, *WhoCanRegister* etkinleştirilir ve **EveryoneInCompany olarak ayarlanır.**</span><span class="sxs-lookup"><span data-stu-id="2ba2b-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="2ba2b-106">Anonim kullanıcılar dahil herkesin kaydolmasına izin vermek için,  Powershell komutunu kullanarak Toplantı İlkesini Herkes olarak ayarlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="2ba2b-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="2ba2b-107">**Not:** Toplantı ayarlarında anonim katılma kapalı ise, anonim kullanıcılar web seminerine kat değildir.</span><span class="sxs-lookup"><span data-stu-id="2ba2b-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="2ba2b-108">Daha fazla bilgi edinmek ve bu ayarı etkinleştirmek için [bkz.](/microsoftteams/meeting-settings-in-teams)Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2ba2b-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="2ba2b-109">Toplantı kaydını kapatmak için *AllowMeetingRegistration'i* False olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="2ba2b-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2ba2b-110">Web seminerleri için kimlerin kaydol etkiyiyi yapılandırma hakkında daha fazla bilgi edinmek için bkz. [Web seminerleri için kimlerin kaydol etkiyi yapılandır?](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="2ba2b-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2ba2b-111">Microsoft Listeleri ayarları hakkında daha fazla bilgi için bkz. [Microsoft Listeleri için ayarları denetleme.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="2ba2b-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
