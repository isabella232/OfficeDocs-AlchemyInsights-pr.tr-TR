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
# <a name="restore-a-deleted-public-folder"></a>Silinmiş ortak klasörü geri yükleme

**Silinmiş öğeleri ortak klasörden geri yüklemek için**:

- [Outlook 2016 'de posta olmayan ortak bir klasörden silinmiş öğeleri kurtaramıyorum](https://aka.ms/pfrec)konusuna bakın.
 
**Silinmiş ortak klasörü geri yüklemek için (herhangi bir tür)**: 

- Lütfen aşağıdaki EXO PowerShell komutunu kullanın:

    İndeki

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Örnek: aşağıdaki komut Subfolder1 'i geri yükler ve \Parent1 altına yerleştirir:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Daha fazla ayrıntı için [Silinmiş ortak klasörü geri yükleme](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) bölümüne bakın.
