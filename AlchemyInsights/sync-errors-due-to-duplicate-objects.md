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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708082"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Yinelenen nesneler nedeniyle eşitleme hataları

Microsoft 365'te dizin eşitlemesi sona geldiğinde aşağıdaki hata iletilerinden birini alabilirsiniz:

- Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler yerel dizininizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerleri olduğundan, bu nesne Microsoft Online Services'ta güncelleştirilemiyor.

- Microsoft Online Services dizininizin içinde aynı proxy adresine sahip eşitlenmiş bir nesne zaten var.

- Bu nesneyle ilişkilendirilmiş aşağıdaki öznitelikler, yerel dizin hizmetlerinizin başka bir nesnesiyle zaten ilişkilendirilmiş olabilir değerleri olduğundan bu nesne güncelleştirilemiyor: UserPrincipalName.

Sorunu tanımlamak ve düzeltmek için IdFix DirSync Hata Düzeltme [Aracı'nı indirin ve çalıştırın.](https://github.com/Microsoft/idfix)

Daha fazla bilgi için [bkz. KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
