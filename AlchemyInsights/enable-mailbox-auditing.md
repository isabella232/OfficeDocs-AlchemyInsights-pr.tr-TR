---
title: Posta kutusu denetimini etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736273"
---
# <a name="enable-mailbox-auditing"></a>Posta kutusu denetimini etkinleştirme

Tek bir kullanıcı veya tüm kuruluş için Posta Kutusu Denetimi'ni etkinleştirmek için Aşağıdaki cmdlets Remote Power Shell'den çalıştırılmalıdır:
  
 **Tek Kullanıcı**
  
Set-Mailbox -Kimlik "Jane Dow" -AuditEnabled $true
  
 **Organizasyon**
  
Get-Mailbox -ResultSize Sınırsız -Filtre {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Daha fazla bilgi edinin](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

