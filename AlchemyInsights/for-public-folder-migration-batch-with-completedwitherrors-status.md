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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158645"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Tamamlanmış Hatalar durumu olan Ortak klasör geçişi için

Büyük/kötü öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın: 
1. Geçiş toplu iş üzerinde atlanan öğeleri onaylayın:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. "Eşitlenen" ancak tamamlanmamış geçiş isteklerinde atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Geçiş toplu işlemi ve istekleri birkaç dakika içinde devam etmeli ve tamamlanmalıdır.

