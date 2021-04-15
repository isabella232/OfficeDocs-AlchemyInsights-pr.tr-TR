---
title: UPN eşitlemesi devre dışı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782171"
---
# <a name="upn-sync-disabled"></a>UPN eşitlemesi devre dışı

Azure AD'ye eşitlemeyi 30 Mart 2016'dan önce başlattıysanız, yalnızca sizin için UPN yumuşak eşleşmesini etkinleştirmek için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
30 Mart 2016'da veya bundan sonra Azure AD'ye eşitlemeye başlayan kuruluşlarda UPN yumuşak eşleşmesi otomatik olarak açılır.
  
UPN'de ve diğer eşitleme özellikleriyle yumuşak eşleşmeyi etkinleştirme hakkında daha fazla bilgi edinmek için bkz. [Azure AD Connect eşitleme hizmeti özellikleri.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

