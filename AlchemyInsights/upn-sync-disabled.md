---
title: UPN eşitlemesi devre dışı bırakıldı
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749534"
---
# <a name="upn-sync-disabled"></a>UPN eşitlemesi devre dışı bırakıldı

30 Mart 2016 tarihinden önce Azure AD ile eşitleme işlemini başlattıysanız, yalnızca kuruluşunuzda UPN kolay eşleşmesinden etkinleştirmek için aşağıdaki Azure AD PowerShell cmdlet 'ini çalıştırın:
  
 **Set-MsolDirSyncFeature-Feature Enablesoftmatch, UPN-Enable $True**
  
%30 Mart 2016 tarihinde veya sonrasında Azure AD 'e eşitlemeyi Başlatan kuruluşlar için UPN yazılımdan eşleşme otomatik olarak açıktır.
  
UPN ve diğer eşitleme özelliklerinde yazılımla eşleştirmeyi etkinleştirme hakkında daha fazla bilgi edinmek için lütfen [Azure AD Connect eşitleme hizmeti özelliklerine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)bakın.
  

