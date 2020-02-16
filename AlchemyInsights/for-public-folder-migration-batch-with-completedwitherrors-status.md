---
title: Tamamlanmış Hatalar durumu olan Ortak klasör geçişi için
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043627"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Tamamlanmış Hatalar durumu olan Ortak klasör geçişi için

Büyük/kötü öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın: 
1. Geçiş toplu iş üzerinde atlanan öğeleri onaylayın:

    Set-MigrationBatch \<batchname> -ApproveSkippedItems 
2. "Eşitlenen" ancak tamamlanmamış geçiş isteklerinde atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($pf $i) {if ($i.LargeItemsEncountered -gt 0 veya $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]:UtcNow)}}
3. Geçiş toplu işlemi ve istekleri birkaç dakika içinde devam etmeli ve tamamlanmalıdır.

