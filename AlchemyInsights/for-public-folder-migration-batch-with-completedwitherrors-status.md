---
title: CompletedWithErrors durumuyla ortak klasör geçiş toplu işlemi
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744133"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors durumuyla ortak klasör geçiş toplu işlemi

Büyük/bozuk öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın: 
1. Geçiş toplu işleminde Atlanan öğeleri onaylama:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. "Eşitlenmiş" Ancak tamamlanmamış geçiş isteklerindeki Atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Geçiş toplu işlemi ve isteklerinin birkaç dakika içinde sürdürülmesi ve tamamlanması gerekir.

