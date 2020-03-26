---
title: Teams istemcisinde takvim simgesi gösterilmiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932381"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Teams istemcisinde takvim simgesi gösterilmiyor

Teams’teki Takvim Sekmesi Exchange Web Hizmetleri aracılığıyla Exchange posta kutusuna erişim gerektirir. Exchange posta kutusu Çevrimiçi veya Şirket İçi olabilir. Takvim Sekmesini görmeyen Çevrimiçi kullanıcıların [Exchange Online posta kutusu lisansına sahip olduklarından ve posta kutusunun etkin olduğundan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) emin olun.

Kullanıcının Exchange Online'da geçerli bir posta kutusu varsa, ancak Takvim sekmesini yine de göremiyorsa, bir ağ sorunuyla karşılaşmış olabilirsiniz. [Microsoft Uzaktan Bağlantı Çözümleyicisi](https://testconnectivity.microsoft.com/)’ni kullanın, etkilenen kullanıcı için **Microsoft Exchange Web Hizmetleri Bağlantı Testleri**’ni çalıştırın.

Son olarak, Takvim uygulamasının kullanıcıya uygulanan ilkeden (büyük olasılıkla **Global (Kuruluş genelinde varsayılan)**’den) kaldırılmadığından emin olmak için [Teams Uygulaması’nın Uygulama kurulum ilkelerini](https://admin.teams.microsoft.com/policies/app-setup) denetleyin.

Kullanıcılarınız Şirket İçinde yerleşikse, Karma yapılandırmanızın sağlıklı olduğundan emin olmalısınız. Sorunu gidermek için [Karma Yapılandırma Sihirbazı](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)’nı kullanın.

[Teams’in Exchange 2016 CU3 veya üzerini gerektirdiğini](https://docs.microsoft.com/microsoftteams/exchange-teams-interact) unutmayın.
