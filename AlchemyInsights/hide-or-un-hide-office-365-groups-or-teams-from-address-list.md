---
title: Adres listesinde grup veya Office 365 gizleme veya gizlemeyi gösterme
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
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088416"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Adres listesinde grup veya Office 365 gizleme veya gizlemeyi gösterme

grup/ekipler grubunu Exchange istemcilerinin (Outlook, OWA) adres listelerinde (GAL) gizlemek veya gizlemek için aşağıdaki EXO Power Office 365 Shell komutunu kullanın:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Office365 grubunu/ekiplerini Exchange istemcilerinden (OWA) gizlemek veya gizlemek için aşağıdaki EXO PowerShell Outlook kullanın:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Ayrıntılı yönergeler için [bkz. Office 365 Grupları GAL ve grup istemcilerinden Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
