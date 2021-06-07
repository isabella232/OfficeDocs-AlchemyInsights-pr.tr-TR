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
# <a name="manage-webinar-registration"></a>Web ziyareti kaydını yönetme

Web seminerleri için kimlerin Teams Powershell komutlarını Teams yönetirsiniz. Powershell'Teams yüklemek için bkz. [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Varsayılan olarak, *WhoCanRegister* etkinleştirilir ve **EveryoneInCompany olarak ayarlanır.** Anonim kullanıcılar dahil herkesin kaydolmasına izin vermek için,  Powershell komutunu kullanarak Toplantı İlkesini Herkes olarak ayarlayabilirsiniz:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Not:** Toplantı ayarlarında anonim katılma kapalı ise, anonim kullanıcılar web seminerine kat değildir. Daha fazla bilgi edinmek ve bu ayarı etkinleştirmek için [bkz.](/microsoftteams/meeting-settings-in-teams)Microsoft Teams.

Toplantı kaydını kapatmak için *AllowMeetingRegistration'i* False olarak **ayarlayın.**

Web seminerleri için kimlerin kaydol etkiyiyi yapılandırma hakkında daha fazla bilgi edinmek için bkz. [Web seminerleri için kimlerin kaydol etkiyi yapılandır?](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Microsoft Listeleri ayarları hakkında daha fazla bilgi için bkz. [Microsoft Listeleri için ayarları denetleme.](/sharepoint/control-lists)
