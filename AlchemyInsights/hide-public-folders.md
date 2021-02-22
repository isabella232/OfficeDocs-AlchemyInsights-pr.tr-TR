---
title: Ortak klasörleri gizleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315443"
---
# <a name="hide-public-folders"></a><span data-ttu-id="b1561-102">Ortak klasörleri gizleme</span><span class="sxs-lookup"><span data-stu-id="b1561-102">Hide public folders</span></span>

<span data-ttu-id="b1561-103">**Ortak klasör ağacının tamamını gizlemek için:**</span><span class="sxs-lookup"><span data-stu-id="b1561-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="b1561-104">Seçmeli klasör ağacının [tamamını veya](https://aka.ms/ControlPF) tüm kullanıcıları gizlemek için bu makaledeki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="b1561-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="b1561-105">**Belirli bir ortak klasörü gizlemek için:**</span><span class="sxs-lookup"><span data-stu-id="b1561-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="b1561-106">Ortak klasöre erişmesi gereken kullanıcılar için izin ekleme</span><span class="sxs-lookup"><span data-stu-id="b1561-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="b1561-107">İzin **listesinden Varsayılan** kullanıcı **kaldırma:**</span><span class="sxs-lookup"><span data-stu-id="b1561-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
