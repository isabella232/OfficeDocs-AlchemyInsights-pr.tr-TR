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
# <a name="hide-public-folders"></a>Ortak klasörleri gizleme

**Ortak klasör ağacının tamamını gizlemek için:**

Seçmeli klasör ağacının [tamamını veya](https://aka.ms/ControlPF) tüm kullanıcıları gizlemek için bu makaledeki adımları kullanın.

**Belirli bir ortak klasörü gizlemek için:**

1. Ortak klasöre erişmesi gereken kullanıcılar için izin ekleme

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. İzin **listesinden Varsayılan** kullanıcı **kaldırma:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
