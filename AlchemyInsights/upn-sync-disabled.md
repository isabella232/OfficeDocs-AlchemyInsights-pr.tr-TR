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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038132"
---
# <a name="upn-sync-disabled"></a>UPN eşitlemesi devre dışı

Azure AD'ye eşitlemeyi 30 Mart 2016'dan önce başlattıysanız, yalnızca sizin için UPN yumuşak eşleşmesini etkinleştirmek için aşağıdaki Azure AD PowerShell cmdlet'ini çalıştırın:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
30 Mart 2016'da veya bundan sonra Azure AD'ye eşitlemeye başlayan kuruluşlarda UPN yumuşak eşleşmesi otomatik olarak açılır.
  
UPN ve diğer eşitleme özellikleri üzerinde yumuşak eşleşmeyi etkinleştirme hakkında daha fazla bilgi edinmek için lütfen [bkz. Azure AD Bağlan eşitleme hizmeti özellikleri.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

