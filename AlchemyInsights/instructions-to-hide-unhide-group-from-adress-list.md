---
title: Grup listesinden grup gizleme/gizleme yönergeleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663029"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365 grubunu adres listesinden gizle (GAL)

Outlook veya OWA gibi bir Microsoft 365 grubunu Adres listelerinden (GAL) gizlemek için, EXO kabuğu 'nda aşağıdaki komutu kullanın:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 grubunu Exchange istemcilerinde görünmemesini gizlemek için, EXO kabuğu 'nda aşağıdaki komutu kullanın:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

