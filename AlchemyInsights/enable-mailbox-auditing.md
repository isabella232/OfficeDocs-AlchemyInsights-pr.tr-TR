---
title: Posta kutusu denetimini etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806311"
---
# <a name="enable-mailbox-auditing"></a>Posta kutusu denetimini etkinleştirme

Tek bir kullanıcı veya kuruluşun tamamında posta kutusu denetimini etkinleştirmek için, aşağıdaki cmdlet 'lerin uzak Power Shell 'den çalıştırılması gerekir:
  
 **Tek Kullanıcı**
  
Set-Mailbox-Identity "Gamze"-Sestenabled $true
  
 **Kuruluşunu**
  
Get-posta kutusu-ResultSize Sınırsız filtre {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-Sestenabled $true
  
[Daha fazla bilgi edinin](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

