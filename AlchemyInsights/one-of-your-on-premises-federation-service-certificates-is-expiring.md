---
title: Şirket içi Federasyon Hizmeti sertifikalarınızdan birinin süresi sona eriyor
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673517"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="bd6b6-102">Şirket içi Federasyon Hizmeti sertifikalarınızdan birinin süresi sona eriyor</span><span class="sxs-lookup"><span data-stu-id="bd6b6-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="bd6b6-103">Bu sorunu çözmek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="bd6b6-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="bd6b6-104">Bilgisayarda Windows PowerShell için Microsoft Azure Active Directory modülünü yükleme (modül yüklü değilse).</span><span class="sxs-lookup"><span data-stu-id="bd6b6-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="bd6b6-105">Bunu yapmak için, [Graph Için Azure Active Directory PowerShell](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) 'e gidin</span><span class="sxs-lookup"><span data-stu-id="bd6b6-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="bd6b6-106">[Federe kullanıcı Microsoft 365, Azure veya Intune 'da oturum AÇTıĞıNDA AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)'Deki "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="bd6b6-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="bd6b6-107">[Microsoft 365, Azure veya Intune 'da federe bir etki alanının ayarlarını güncelleştirme veya onarma ile ilgili](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="bd6b6-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="bd6b6-108">Federasyon sertifikalarını yenileme hakkında daha fazla bilgi için [O365 ve Azure AD Için sertifika yenileme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="bd6b6-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

