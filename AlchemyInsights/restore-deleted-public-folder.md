---
title: Silinmiş ortak klasörü geri yükleme
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774551"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="ab645-102">Silinmiş ortak klasörü geri yükleme</span><span class="sxs-lookup"><span data-stu-id="ab645-102">Restore a deleted public folder</span></span>

<span data-ttu-id="ab645-103">**Silinmiş öğeleri ortak klasörden geri yüklemek için**:</span><span class="sxs-lookup"><span data-stu-id="ab645-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="ab645-104">[Outlook 2016 'de posta olmayan ortak bir klasörden silinmiş öğeleri kurtaramıyorum](https://aka.ms/pfrec)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="ab645-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="ab645-105">**Silinmiş ortak klasörü geri yüklemek için (herhangi bir tür)**:</span><span class="sxs-lookup"><span data-stu-id="ab645-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="ab645-106">Lütfen aşağıdaki EXO PowerShell komutunu kullanın:</span><span class="sxs-lookup"><span data-stu-id="ab645-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="ab645-107">İndeki</span><span class="sxs-lookup"><span data-stu-id="ab645-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="ab645-108">Örnek: aşağıdaki komut Subfolder1 'i geri yükler ve \Parent1 altına yerleştirir:</span><span class="sxs-lookup"><span data-stu-id="ab645-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="ab645-109">Daha fazla ayrıntı için [Silinmiş ortak klasörü geri yükleme](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="ab645-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
