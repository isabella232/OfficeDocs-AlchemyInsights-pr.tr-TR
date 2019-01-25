---
title: Şirket içi Federasyon Hizmeti sertifikalarınızı birini süresinin dolmasını
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494454"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="2f811-102">Şirket içi Federasyon Hizmeti sertifikalarınızı birini süresinin dolmasını</span><span class="sxs-lookup"><span data-stu-id="2f811-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="2f811-103">Bu sorunu gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="2f811-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="2f811-p101">Microsoft Azure Active Directory modülü için Windows PowerShell (modül yüklü değil ise) bilgisayara yükleyin. Bunu yapmak için [Grafik için Active Directory PowerShell Azure](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) gidin.</span><span class="sxs-lookup"><span data-stu-id="2f811-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="2f811-106">Adımları "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümünde [Office 365, Azure veya Intune federe bir kullanıcı oturum açtığında AD FS "sitesine erişilirken bir sorun oluştu" hata](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="2f811-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="2f811-107">T[nasıl update veya Office 365, Azure, veya Intune bir federe etki alanı ayarlarını onarmak](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2f811-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="2f811-108">Federasyon sertifikaları yenileme hakkında daha fazla bilgi için bkz: [sertifika yenilemesi için O365 ve Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="2f811-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

