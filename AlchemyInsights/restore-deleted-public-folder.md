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
# <a name="restore-a-deleted-public-folder"></a>Silinen ortak klasörü geri yükleme

**Ortak klasörden silinen öğeleri geri yüklemek için:**

- Bkz. [Outlook 2016'da silinen öğeleri posta olmayan bir ortak klasörden kurtaramazsınız.](https://aka.ms/pfrec)
 
**Silinen ortak klasörü (herhangi bir türde) geri yüklemek için:** 

- Lütfen aşağıdaki EXO PowerShell komutunu kullanın:

    Sözdizimi:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | | {$_. Ad -eq\<" name_of_deleted_public_Folder"}; Klasörü> geri yüklenecek \<olan Yol $pf.Identity -Yol yolunu

    Örnek: Aşağıdaki komut Alt Klasör1'i geri yükleyecek ve \Parent1 altına yerleştirilecektir:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | | {$_. Ad -eq "Alt klasör1"}; Set-PublicFolder $pf.identity -Yol \Parent1

Bkz. Daha fazla ayrıntı için [silinen ortak klasörü geri yükleyin.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
