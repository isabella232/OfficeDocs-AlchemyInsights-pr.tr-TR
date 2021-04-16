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
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810072"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Şirket içi Federasyon Hizmeti Sertifikalarından birinin süresi dolmak üzere

Bu sorunu çözmek için şu adımları izleyin:
  
- Windows PowerShell için Microsoft Azure Active Directory Modülü'ne (modül zaten yüklü değilse) yükleyin. Bunu yapmak için [Azure Active Directory PowerShell for Graph'e gidin ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Federasyon kullanıcısı [Microsoft 365, Azure veya Intune'da](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oturum adiğinde AD FS'den alınan "Siteye erişimle ilgili bir sorun oluştu" hatasının "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.
    
- [Microsoft 365, Azure veya Intune'da](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)federasyon etki alanının ayarlarını güncelleştirme veya onarma makalesinde yer alan adımları izleyin.
    
Federasyon sertifikalarını yenileme hakkında daha fazla bilgi için bkz. [O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)ve Azure AD için sertifika yenileme.
  

