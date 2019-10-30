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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768960"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Adres listesinden Office 365 grubunu gizle (GAL)

Bir Office 365 grubunu Exchange istemcilerinin adres listelerinden (GAL) gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Office 365 grubunu Exchange istemcilerine görünür olmasını gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

