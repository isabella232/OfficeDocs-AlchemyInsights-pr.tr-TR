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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="e0e66-102">Tamamlanmış Hatalar durumu olan Ortak klasör geçişi için</span><span class="sxs-lookup"><span data-stu-id="e0e66-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="e0e66-103">Büyük/kötü öğeleri atlayarak toplu işlemi tamamlamak için aşağıdaki adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="e0e66-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="e0e66-104">Geçiş toplu iş üzerinde atlanan öğeleri onaylayın:</span><span class="sxs-lookup"><span data-stu-id="e0e66-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="e0e66-105">"Eşitlenen" ancak tamamlanmamış geçiş isteklerinde atlanan öğeleri onaylamak için aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="e0e66-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="e0e66-106">Geçiş toplu işlemi ve istekleri birkaç dakika içinde devam etmeli ve tamamlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="e0e66-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

