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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737209"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9e47b-102">ADFS Federasyon Sertifikası Süresi Doluyor</span><span class="sxs-lookup"><span data-stu-id="9e47b-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9e47b-103">Bu sorunu gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="9e47b-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9e47b-104">Windows PowerShell için Microsoft Azure Active Directory Modül'ü bilgisayara yükleyin (modül zaten yüklü değilse).</span><span class="sxs-lookup"><span data-stu-id="9e47b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="9e47b-105">Bunu yapmak için [Windows PowerShell'i kullanarak Azure REKLAM'ı yönet'e](https://aka.ms/aadposh)gidin.</span><span class="sxs-lookup"><span data-stu-id="9e47b-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="9e47b-106">Federe [bir kullanıcı Office 365, Azure veya Intune'a girdiğinde AD FS'den gelen "Siteye erişimde sorun oluştu" bölümünün](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)"Senaryo 1: AD FS belirteç imzalama sertifikasının süresi doldu" bölümündeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="9e47b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="9e47b-107">[Office 365, Azure veya Intune'daki federe etki alanının ayarlarını güncelleştirme veya onarma](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)adımlarını izleyin.</span><span class="sxs-lookup"><span data-stu-id="9e47b-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="9e47b-108">Federasyon sertifikalarını yenileme hakkında daha fazla bilgi edinmek [için Office 365 ve Azure Etkin Dizini için federasyon sertifikalarını](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)yenile'ye bakın.</span><span class="sxs-lookup"><span data-stu-id="9e47b-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
