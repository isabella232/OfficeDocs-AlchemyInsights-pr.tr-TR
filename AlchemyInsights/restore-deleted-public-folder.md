---
title: Silinen ortak klasörü geri yükleme
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063772"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="65088-102">Silinen ortak klasörü geri yükleme</span><span class="sxs-lookup"><span data-stu-id="65088-102">Restore a deleted public folder</span></span>

<span data-ttu-id="65088-103">**Ortak klasörden silinen öğeleri geri yüklemek için:**</span><span class="sxs-lookup"><span data-stu-id="65088-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="65088-104">Bkz. [Outlook 2016'da silinen öğeleri posta olmayan bir ortak klasörden kurtaramazsınız.](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="65088-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="65088-105">**Silinen ortak klasörü (herhangi bir türde) geri yüklemek için:**</span><span class="sxs-lookup"><span data-stu-id="65088-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="65088-106">Lütfen aşağıdaki EXO PowerShell komutunu kullanın:</span><span class="sxs-lookup"><span data-stu-id="65088-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="65088-107">Sözdizimi:</span><span class="sxs-lookup"><span data-stu-id="65088-107">Syntax:</span></span>

    ><span data-ttu-id="65088-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | | {$_. Ad -eq\<" name_of_deleted_public_Folder"}; Klasörü> geri yüklenecek \<olan Yol $pf.Identity -Yol yolunu</span><span class="sxs-lookup"><span data-stu-id="65088-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="65088-109">Örnek: Aşağıdaki komut Alt Klasör1'i geri yükleyecek ve \Parent1 altına yerleştirilecektir:</span><span class="sxs-lookup"><span data-stu-id="65088-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="65088-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | | {$_. Ad -eq "Alt klasör1"}; Set-PublicFolder $pf.identity -Yol \Parent1</span><span class="sxs-lookup"><span data-stu-id="65088-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="65088-111">Bkz. Daha fazla ayrıntı için [silinen ortak klasörü geri yükleyin.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)</span><span class="sxs-lookup"><span data-stu-id="65088-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
