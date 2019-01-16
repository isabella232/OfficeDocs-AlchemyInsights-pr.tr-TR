---
title: Posta kutusu denetimi etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317338"
---
# <a name="enable-mailbox-auditing"></a>Posta kutusu denetimi etkinleştirme

Tek bir kullanıcı veya tüm kuruluş için posta kutusu denetimini etkinleştirmek için aşağıdaki cmdlet'leri uzak güç kabuğundan çalıştırmanız gerekir:
  
 **Tek kullanıcı**
  
Set-posta kutusu - kimlik "Jane Dow" - AuditEnabled $true
  
 **Kuruluş**
  
Get-posta kutusu - ResultSize sınırsız - filtre {RecipientTypeDetails - eq "UserMailbox"} | Set-posta kutusu - AuditEnabled $true
  
[Daha fazla bilgi edinin](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

