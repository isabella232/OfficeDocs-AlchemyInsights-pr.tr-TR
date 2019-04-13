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
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859124"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Eşitleme hataları nedeniyle nesneleri çoğaltma

Dizin eşitleme tamamlandığında, aşağıdaki hata iletilerinden birini alabilirsiniz:

- Bu Microsoft Çevrimiçi Hizmetler nesnesinde zaten yerel dizin başka bir nesneyle ilişkilendirilmiş olan değerlerini Bu nesneyle ilişkili aşağıdaki özniteliklere sahip olduğundan güncelleştirilemedi.

- Microsoft Çevrimiçi Hizmetler dizininizde proxy adresi ile eşitlenmiş bir nesne zaten var.

- Bu nesne zaten, yerel dizin hizmetlerinde başka bir nesne ile ilişkili olabilir değerleri Bu nesneyle ilişkili aşağıdaki özniteliklere sahip olduğundan güncelleştirilemedi: UserPrincipalName.

Sorunu tanımlamak ve gidermek için karşıdan yükleme ve [IdFix DirSync hata düzeltme aracı](https://www.microsoft.com/download/details.aspx?id=36832)' nı çalıştırın.

Daha fazla bilgi için bkz: [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
