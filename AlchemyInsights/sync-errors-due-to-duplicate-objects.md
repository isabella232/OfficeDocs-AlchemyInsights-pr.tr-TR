---
title: 902 (Yinelenen nesneler nedeniyle oluşan eşitleme hataları)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998820"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Yinelenen nesneler nedeniyle eşitleme hataları

Dizin eşitlemesi son olarak aşağıdaki hata iletilerinden birini Microsoft 365:

- Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler, yerel dizininizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerlerine sahip olduğundan, bu nesne Microsoft Online Services'ta güncelleştirilemiyor.

- Microsoft Online Services dizininizin içinde aynı ara sunucu adresine sahip eşitlenmiş bir nesne var.

- Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler, yerel dizin hizmetlerinizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerlerine sahip olduğundan, bu nesne güncelleştirilemiyor: UserPrincipalName.

Sorunu tanımlamak ve düzeltmek için [IdFix DirSync Hata Düzeltme Aracı'nı indirip çalıştırın.](https://github.com/Microsoft/idfix)

Daha fazla bilgi için [bkz. KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
