---
title: Grubu adres listesinde gizleme/gösterme yönergeleri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926265"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Adres Microsoft 365 (GAL) grubunu gizleme

Bir Microsoft 365 istemcilerinin adres listelerinde (GAL) Exchange (Outlook veya OWA gibi) gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Dış istemcilerde Microsoft 365 görünür durumdan Exchange EXO kabuğunda aşağıdaki komutu kullanın:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

