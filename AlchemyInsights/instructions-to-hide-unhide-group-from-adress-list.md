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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="ee4cb-102">Microsoft 365 grubunu adres listesinden gizleme (GAL)</span><span class="sxs-lookup"><span data-stu-id="ee4cb-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="ee4cb-103">Microsoft 365 grubunu Exchange istemcilerinin adres listelerinden (GAL) gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="ee4cb-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="ee4cb-104">Microsoft 365 grubunu Exchange istemcilerine görünür olmasını gizlemek için EXO kabuğunda aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="ee4cb-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

