---
title: Silinmiş ortak klasörü geri yükleme
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809459"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="46612-102">Silinmiş ortak klasörü geri yükleme</span><span class="sxs-lookup"><span data-stu-id="46612-102">Restore a deleted public folder</span></span>

<span data-ttu-id="46612-103">**Silinmiş öğeleri ortak klasörden geri yüklemek için:**</span><span class="sxs-lookup"><span data-stu-id="46612-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="46612-104">Bkz. [Outlook 2016'da](https://aka.ms/pfrec)posta dışında bir ortak klasörden silinmiş öğeleri kurtarasınız.</span><span class="sxs-lookup"><span data-stu-id="46612-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="46612-105">**Silinmiş bir ortak klasörü (her tür) geri yüklemek için:**</span><span class="sxs-lookup"><span data-stu-id="46612-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="46612-106">Lütfen aşağıdaki EXO PowerShell komutunu kullanın:</span><span class="sxs-lookup"><span data-stu-id="46612-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="46612-107">Söz dizimi:</span><span class="sxs-lookup"><span data-stu-id="46612-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="46612-108">Örnek: Aşağıdaki komut Alt Klasör1'i geri yükle ve \Parent1 altına gelecektir:</span><span class="sxs-lookup"><span data-stu-id="46612-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="46612-109">Daha [fazla bilgi için bkz. Silinmiş bir ortak](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) klasörü geri yükleme.</span><span class="sxs-lookup"><span data-stu-id="46612-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
