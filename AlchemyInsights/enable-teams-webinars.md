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
# <a name="enable-teams-webinars"></a>Web seminerlerini Teams etkinleştirme

Web seminerleri varsayılan olarak etkindir. Teams PowerShell komutlarını kullanarak, Web seminerleri için kimlerin zaman Teams kaydola bir şekilde yönetebilirsiniz.

- Toplantı oluşturan tüm kullanıcılar, web amaçlı toplantı da oluşturabilir. Web seminerleri için kimlerin zaman Teams yönetmek için *AllowMeetingRegistration kullanın.* 
- Varsayılan olarak, *WhoCanRegister* etkindir ve Herkes olarak **ayarlanır.** Toplantı kaydını kapatmak için *AllowMeetingRegistration'i* False olarak **ayarlayın.**

Bu ayarları değiştirmek için, Teams [PowerShell yüklemeniz gerekir.](/microsoftteams/teams-powershell-install) Ayrıca, Toplantı İlkeleri web seminerleri Teams uygulanır. Örneğin, toplantı ayarlarında anonim katılma kapalı ise, anonim kullanıcılar web seminerine kat değildir.

Web seminerleri için kimlerin kaydol etkiyiyi yapılandırma hakkında daha fazla bilgi edinmek için bkz. [Web seminerleri için kimlerin kaydol etkiyi yapılandır?](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Microsoft Listeleri ayarları hakkında daha fazla bilgi için bkz. [Microsoft Listeleri için ayarları denetleme.](/sharepoint/control-lists)