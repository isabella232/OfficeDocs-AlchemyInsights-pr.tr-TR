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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068184"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors durumunu içeren Ortak klasör geçiş toplu işlemi için

Büyük/kötü öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın: 
1. Geçiş toplu işlemi sırasında atlanan öğeleri onaylama:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. "Eşitleniyor" olan ancak tamamlanmadı olan geçiş isteklerinde atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Geçiş toplu işleminin ve isteklerinin birkaç dakika içinde devam etmesi ve tamamlanması gerekir.

