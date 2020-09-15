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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="0f7bb-102">Microsoft 365 grubunu adres listesinden gizle (GAL)</span><span class="sxs-lookup"><span data-stu-id="0f7bb-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="0f7bb-103">Outlook veya OWA gibi bir Microsoft 365 grubunu Adres listelerinden (GAL) gizlemek için, EXO kabuğu 'nda aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="0f7bb-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="0f7bb-104">Microsoft 365 grubunu Exchange istemcilerinde görünmemesini gizlemek için, EXO kabuğu 'nda aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="0f7bb-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

