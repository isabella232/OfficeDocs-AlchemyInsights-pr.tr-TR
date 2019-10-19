---
title: ADFS Federasyon Sertifikası Süresi Doluyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737209"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federasyon Sertifikası Süresi Doluyor

Bu sorunu gidermek için aşağıdaki adımları izleyin:
  
1. Windows PowerShell için Microsoft Azure Active Directory Modül'ü bilgisayara yükleyin (modül zaten yüklü değilse). Bunu yapmak için [Windows PowerShell'i kullanarak Azure REKLAM'ı yönet'e](https://aka.ms/aadposh)gidin.

2. Federe [bir kullanıcı Office 365, Azure veya Intune'a girdiğinde AD FS'den gelen "Siteye erişimde sorun oluştu" bölümünün](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)"Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.

3. [Office 365, Azure veya Intune'daki federe etki alanının ayarlarını güncelleştirme veya onarma](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)adımlarını izleyin.

    Federasyon sertifikalarını yenileme hakkında daha fazla bilgi edinmek [için Office 365 ve Azure Etkin Dizini için federasyon sertifikalarını](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)yenile'ye bakın.
