---
title: ADFS Federasyon sertifika zaman aşımına uğramak
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398360"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federasyon sertifika zaman aşımına uğramak

Bu sorunu gidermek için şu adımları izleyin:
  
1. Microsoft Azure Active Directory modülü için Windows PowerShell (modül yüklü değil ise) bilgisayara yükleyin. Bunu yapmak için [Windows PowerShell kullanarak Azure AD Yönet](https://aka.ms/aadposh)gidin.
    
2. Adımları "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümünde [Office 365, Azure veya Intune federe bir kullanıcı oturum açtığında AD FS "sitesine erişilirken bir sorun oluştu" hata](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. [Nasıl update veya Office 365, Azure, veya Intune bir federe etki alanı ayarlarını onarmak](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)adımları izleyin.
    
    Federasyon sertifikaları yenileme hakkında daha fazla bilgi için bkz: [Office 365 ve Azure Active Directory Federasyon sertifikalarını yenileme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

