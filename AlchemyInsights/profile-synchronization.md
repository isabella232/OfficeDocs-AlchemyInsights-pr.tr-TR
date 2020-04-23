---
title: Profil eşitleme
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768133"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Profilim ne zaman SharePoint Kullanıcı Profili Uygulamasıile senkronize olur?

SharePoint Online, kullanıcıları ve grupları Kullanıcı Profili Uygulamasına aktarmak için Active Directory Import timer işini (AD Alma) kullanır. 
  
1. AD Alma, SharePoint Online Directory Store'dan Kullanıcı Profili Uygulamasına değişiklikleri eşitler. Bu değişiklikler toplu olarak işlenir.
    
2. Zamanlayıcı işi, değişiklikler eşitlenene kadar çalışır.
    
> [!NOTE]
> İşi çalıştırmak için aldığı süre, işlemdeki değişikliklerin sayısına bağlıdır. Çok sayıda değişiklik daha uzun sürer. Hizmet Düzeyi Sözleşmesi (SLA), SharePoint Online Dizininde bir kullanıcıdeğişikliğinin 24 saat içinde Kullanıcı Profili Uygulamasına yansıyacağını belirtir. 
  
[SharePoint Online kullanıcı profili senkronizasyonu hakkında daha fazla bilgi](https://go.microsoft.com/fwlink/?linkid=875671)
  

