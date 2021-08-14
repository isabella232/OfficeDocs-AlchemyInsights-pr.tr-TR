---
title: Teams istemcisinde takvim simgesi gösterilmiyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989611"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Teams istemcisinde takvim simgesi gösterilmiyor

Teams’teki Takvim Sekmesi Exchange Web Hizmetleri aracılığıyla Exchange posta kutusuna erişim gerektirir. Exchange posta kutusu Çevrimiçi veya Şirket İçi olabilir. Takvim Sekmesini görmeyen Çevrimiçi kullanıcıların [Exchange Online posta kutusu lisansına sahip olduklarından ve posta kutusunun etkin olduğundan](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) emin olun.

Kullanıcının Exchange Online'da geçerli bir posta kutusu varsa, ancak Takvim sekmesini yine de göremiyorsa, bir ağ sorunuyla karşılaşmış olabilirsiniz. [Microsoft Uzaktan Bağlantı Çözümleyicisi](https://testconnectivity.microsoft.com/)’ni kullanın, etkilenen kullanıcı için **Microsoft Exchange Web Hizmetleri Bağlantı Testleri**’ni çalıştırın.

Son olarak, Takvim uygulamasının kullanıcıya uygulanan ilkeden (büyük olasılıkla **Global (Kuruluş genelinde varsayılan)**’den) kaldırılmadığından emin olmak için [Teams Uygulaması’nın Uygulama kurulum ilkelerini](https://admin.teams.microsoft.com/policies/app-setup) denetleyin.

Kullanıcılarınız Şirket İçinde yerleşikse, Karma yapılandırmanızın sağlıklı olduğundan emin olmalısınız. Sorunu gidermek için [Karma Yapılandırma Sihirbazı](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)’nı kullanın.

[Teams’in Exchange 2016 CU3 veya üzerini gerektirdiğini](https://docs.microsoft.com/microsoftteams/exchange-teams-interact) unutmayın.
