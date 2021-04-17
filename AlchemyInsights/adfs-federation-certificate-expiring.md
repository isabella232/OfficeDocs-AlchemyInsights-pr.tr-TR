---
title: ADFS Federasyon Sertifikası Süresi Dolıyor
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821971"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federasyon Sertifikası Süresi Dolıyor

Bu sorunu çözmek için şu adımları izleyin:
  
1. Windows PowerShell için Microsoft Azure Active Directory Modülü'ne (modül zaten yüklü değilse) yükleyin. Bunu yapmak için [Windows PowerShell kullanarak Azure AD'yi yönetme 'ye gidin.](https://aka.ms/aadposh)

2. Federasyon kullanıcısı [Microsoft 365, Azure veya Intune'da](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oturum adiğinde AD FS'den alınan "Siteye erişimle ilgili bir sorun oluştu" hatasının "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.

3. Microsoft, Azure veya [Intune'da](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)federasyon etki alanının ayarlarını güncelleştirme veya onarma'daki adımları izleyin.

    Federasyon sertifikalarını yenileme hakkında daha fazla bilgi edinmek için [bkz. Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)ve Azure Active Directory için federasyon sertifikalarını yenileme.
