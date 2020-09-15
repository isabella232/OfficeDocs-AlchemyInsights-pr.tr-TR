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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9689b-102">ADFS Federasyon sertifikasının süresi doluyor</span><span class="sxs-lookup"><span data-stu-id="9689b-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9689b-103">Bu sorunu çözmek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="9689b-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9689b-104">Bilgisayarda Windows PowerShell için Microsoft Azure Active Directory modülünü yükleme (modül yüklü değilse).</span><span class="sxs-lookup"><span data-stu-id="9689b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="9689b-105">Bunu yapmak için, [Windows PowerShell kullanarak Azure AD 'Yi yönetme](https://aka.ms/aadposh)bölümüne gidin.</span><span class="sxs-lookup"><span data-stu-id="9689b-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="9689b-106">[Federe kullanıcı Microsoft 365, Azure veya Intune 'da oturum AÇTıĞıNDA AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)'Deki "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="9689b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="9689b-107">[Microsoft, Azure veya Intune 'daki Federasyon etki alanının ayarlarını güncelleştirme veya onarma](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)bölümündeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="9689b-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="9689b-108">Federasyon sertifikalarını yenileme hakkında daha fazla bilgi edinmek için, [Microsoft 365 ve Azure Active Directory için Federasyon sertifikalarını yenileme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="9689b-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
