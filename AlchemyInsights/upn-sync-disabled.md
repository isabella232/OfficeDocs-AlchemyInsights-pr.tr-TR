---
title: UPN eşitleme devre dışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423588"
---
# <a name="upn-sync-disabled"></a>UPN eşitleme devre dışı

Eşitlemeden önce 30 Mart 2016 Azure AD için başlatılan yalnızca kuruluşunuz için UPN yumuşak eşleşme sağlamak için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:
  
 **Kümesi-MsolDirSyncFeature-özellik EnableSoftMatchOnUpn-$True etkinleştir**
  
UPN yumuşak eşleşme Azure AD veya daha sonra 30 Mart 2016 için eşitleme başlatıldı organizasyonlar için otomatik olarak etkinleştirilir.
  
Yumuşak eşleşen UPN ve diğer eşitleme özellikleri etkinleştirme hakkında daha fazla bilgi için lütfen [Azure AD Bağlan eşitleme hizmeti özellikleri](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.
  

