---
title: Şirket içi Federasyon Hizmeti Sertifikalarından birinin süresi dolmak üzere
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985237"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Şirket içi Federasyon Hizmeti Sertifikalarından birinin süresi dolmak üzere

Bu sorunu çözmek için şu adımları izleyin:
  
- Bilgisayarınızda Microsoft Azure Active Directory için Windows PowerShell Modülü'ne yükleyin (modül daha önce yüklenmemişse). Bunu yapmak için, Azure Active Directory [PowerShell'i Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Federasyon kullanıcısı Microsoft 365, Azure veya [Intune'da](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oturum adiğinde AD FS'den alınan "Siteye erişimle ilgili bir sorun oluştu" hatasının "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.
    
- Microsoft 365, Azure veya Intune'da federasyon etki alanının ayarlarını güncelleştirme veya onarma [sayfasındaki adımları izleyin.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Federasyon sertifikalarını yenileme hakkında daha fazla bilgi için bkz. [O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)ve Azure AD için sertifika yenileme.
  

