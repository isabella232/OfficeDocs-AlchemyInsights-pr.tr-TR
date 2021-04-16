---
title: CompletedWithErrors durumunu içeren Ortak klasör geçiş toplu işlemi için
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812484"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors durumunu içeren Ortak klasör geçiş toplu işlemi için

Büyük/kötü öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın: 
1. Geçiş toplu işlemi sırasında atlanan öğeleri onaylama:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. "Eşitleniyor" olan ancak tamamlanmadı olan geçiş isteklerinde atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Geçiş toplu işleminin ve isteklerinin birkaç dakika içinde devam etmesi ve tamamlanması gerekir.

