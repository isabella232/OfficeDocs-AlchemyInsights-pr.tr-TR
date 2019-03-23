---
title: 902 (Eşitleme hataları nedeniyle yinelenen nesneleri)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781281"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Eşitleme hataları nedeniyle nesneleri çoğaltma

Dizin eşitleme tamamlandığında, aşağıdaki hata iletilerinden birini alabilirsiniz:
  
- Bu Microsoft Çevrimiçi Hizmetler nesnesinde zaten yerel dizin başka bir nesneyle ilişkilendirilmiş olan değerlerini Bu nesneyle ilişkili aşağıdaki özniteliklere sahip olduğundan güncelleştirilemedi.
    
- Microsoft Çevrimiçi Hizmetler dizininizde proxy adresi ile eşitlenmiş bir nesne zaten var.
    
- Bu nesne zaten, yerel dizin hizmetlerinde başka bir nesne ile ilişkili olabilir değerleri Bu nesneyle ilişkili aşağıdaki özniteliklere sahip olduğundan güncelleştirilemedi: UserPrincipalName.
    
Sorunu tanımlamak ve gidermek için karşıdan yükleme ve [IdFix DirSync hata düzeltme aracı](https://www.microsoft.com/download/details.aspx?id=36832)' nı çalıştırın.
  
Daha fazla bilgi için bkz: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

