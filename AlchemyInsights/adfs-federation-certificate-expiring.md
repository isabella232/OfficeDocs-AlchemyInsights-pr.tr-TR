---
title: ADFS Federasyon sertifikasının süresi doluyor
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686775"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federasyon sertifikasının süresi doluyor

Bu sorunu çözmek için aşağıdaki adımları izleyin:
  
1. Bilgisayarda Windows PowerShell için Microsoft Azure Active Directory modülünü yükleme (modül yüklü değilse). Bunu yapmak için, [Windows PowerShell kullanarak Azure AD 'Yi yönetme](https://aka.ms/aadposh)bölümüne gidin.

2. [Federe kullanıcı Microsoft 365, Azure veya Intune 'da oturum AÇTıĞıNDA AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)'Deki "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.

3. [Microsoft, Azure veya Intune 'daki Federasyon etki alanının ayarlarını güncelleştirme veya onarma](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)bölümündeki adımları izleyin.

    Federasyon sertifikalarını yenileme hakkında daha fazla bilgi edinmek için, [Microsoft 365 ve Azure Active Directory için Federasyon sertifikalarını yenileme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)konusuna bakın.
