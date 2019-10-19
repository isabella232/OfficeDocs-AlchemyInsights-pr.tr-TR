---
title: Profil eşitleme
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554353"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Profilim ne zaman SharePoint Kullanıcı Profili Uygulamasıile senkronize olur?

SharePoint Online, kullanıcıları ve grupları Kullanıcı Profili Uygulamasına aktarmak için Active Directory Import timer işini (AD Alma) kullanır. 
  
1. AD Alma, SharePoint Online Directory Store'dan Kullanıcı Profili Uygulamasına değişiklikleri eşitler. Bu değişiklikler toplu olarak işlenir.
    
2. Zamanlayıcı işi, değişiklikler eşitlenene kadar çalışır.
    
> [!NOTE]
> İşi çalıştırmak için aldığı süre, işlemdeki değişikliklerin sayısına bağlıdır. Çok sayıda değişiklik daha uzun sürer. Hizmet Düzeyi Sözleşmesi (SLA), SharePoint Online Dizininde bir kullanıcıdeğişikliğinin 24 saat içinde Kullanıcı Profili Uygulamasına yansıyacağını belirtir. 
  
[SharePoint Online kullanıcı profili senkronizasyonu hakkında daha fazla bilgi](https://go.microsoft.com/fwlink/?linkid=875671)
  

