---
title: Şirket içi Federasyon Hizmet Sertifikalarınızdan birinin süresi doluyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785323"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Şirket içi Federasyon Hizmet Sertifikalarınızdan birinin süresi doluyor

Bu sorunu gidermek için aşağıdaki adımları izleyin:
  
- Windows PowerShell için Microsoft Azure Active Directory Modül'ü bilgisayara yükleyin (modül zaten yüklü değilse). Bunu yapmak [için, Grafik için Azure Active Directory PowerShell'e](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) gidin
    
- Federe [bir kullanıcı Microsoft 365, Azure veya Intune'a girdiğinde AD FS'den gelen "Siteye erişimde bir sorun vardı" bölümünün](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)"Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.
    
- [Microsoft 365, Azure veya Intune'daki federe bir etki alanının ayarlarını güncelleştirme veya onarma ile ilgili](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)adımları izleyin.
    
Federasyon sertifikalarını yenileme hakkında daha fazla bilgi [için, O365 ve Azure AD için Sertifika yenileme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)adresine bakın.
  

