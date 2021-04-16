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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="f02ba-102">Şirket içi Federasyon Hizmeti Sertifikalarından birinin süresi dolmak üzere</span><span class="sxs-lookup"><span data-stu-id="f02ba-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="f02ba-103">Bu sorunu çözmek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="f02ba-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="f02ba-104">Windows PowerShell için Microsoft Azure Active Directory Modülü'ne (modül zaten yüklü değilse) yükleyin.</span><span class="sxs-lookup"><span data-stu-id="f02ba-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f02ba-105">Bunu yapmak için [Azure Active Directory PowerShell for Graph'e gidin ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f02ba-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="f02ba-106">Federasyon kullanıcısı [Microsoft 365, Azure veya Intune'da](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oturum adiğinde AD FS'den alınan "Siteye erişimle ilgili bir sorun oluştu" hatasının "Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="f02ba-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="f02ba-107">[Microsoft 365, Azure veya Intune'da](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)federasyon etki alanının ayarlarını güncelleştirme veya onarma makalesinde yer alan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="f02ba-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="f02ba-108">Federasyon sertifikalarını yenileme hakkında daha fazla bilgi için bkz. [O365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)ve Azure AD için sertifika yenileme.</span><span class="sxs-lookup"><span data-stu-id="f02ba-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

