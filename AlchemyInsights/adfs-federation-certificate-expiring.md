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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952989"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federasyon Sertifikası Süresi Dolıyor

Bu sorunu çözmek için şu adımları izleyin:
  
1. Bilgisayarınızda Microsoft Azure Active Directory için Windows PowerShell Modülü'ne yükleyin (modül daha önce yüklenmemişse). Bunu yapmak için, [Azure AD'i Windows PowerShell.](https://aka.ms/aadposh)

2. Federasyon kullanıcısı Microsoft 365, Azure veya [Intune'da](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oturum adiğinde AD FS'den alınan "Siteye erişimle ilgili bir sorun oluştu" hatasının "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.

3. Microsoft, Azure veya [Intune'da](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)federasyon etki alanının ayarlarını güncelleştirme veya onarma'daki adımları izleyin.

    Federasyon sertifikalarını yenileme hakkında daha fazla bilgi için bkz. Federasyon sertifikaları [için Microsoft 365 Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
