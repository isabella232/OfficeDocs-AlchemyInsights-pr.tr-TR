---
title: Grubu adres listesinden gizleme/gizleme yönergeleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908364"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365 grubunu adres listesinden gizleme (GAL)

Microsoft 365 grubunu Exchange istemcilerinin adres listelerinden (GAL) gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 grubunu Exchange istemcilerine görünür olmasını gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

