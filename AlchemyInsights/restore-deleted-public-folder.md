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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943395"
---
# <a name="restore-a-deleted-public-folder"></a>Silinmiş ortak klasörü geri yükleme

**Silinmiş öğeleri ortak klasörden geri yüklemek için:**

- Bkz. [bir klasörde postayla ilgili olmayan ortak klasörden silinmiş öğeleri Outlook 2016.](https://aka.ms/pfrec)
 
**Silinmiş bir ortak klasörü (her tür) geri yüklemek için:** 

- Lütfen aşağıdaki EXO PowerShell komutunu kullanın:

    Söz dizimi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Örnek: Aşağıdaki komut Alt Klasör1'i geri yükle ve \Parent1 altına gelecektir:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Daha [fazla bilgi için bkz. Silinmiş bir ortak](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) klasörü geri yükleme.
