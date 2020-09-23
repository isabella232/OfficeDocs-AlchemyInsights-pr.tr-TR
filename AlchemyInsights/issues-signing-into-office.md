---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236145"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="6a641-102">Microsoft 365 uygulamalarında oturum açan sorunlar</span><span class="sxs-lookup"><span data-stu-id="6a641-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="6a641-103">Microsoft 365 uygulamalarıyla oturum açma sorunlarını çözmek için etkilenen makinede aşağıdaki seçenekleri deneyin:</span><span class="sxs-lookup"><span data-stu-id="6a641-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="6a641-104">Windows için, [yaygın oturum açma sorunlarını çözme önerilerine](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) bakın</span><span class="sxs-lookup"><span data-stu-id="6a641-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="6a641-105">Mac için, bkz:  [Mac Için Office 2016 uygulamasında oturum açamıyorum](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="6a641-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="6a641-106">**İpucu** Windows makinelerde, birkaç yaygın Office oturum açma sorununu tanılayabilir ve otomatik olarak düzeltebiliriz.</span><span class="sxs-lookup"><span data-stu-id="6a641-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="6a641-107">Otomatikleştirilmiş hizmetlerimizi kullanmak için  **[Microsoft destek ve Kurtarma Yardımcısı](https://aka.ms/SaRA-OfficeSignInScenario)** 'nı indirin ve kullanın.</span><span class="sxs-lookup"><span data-stu-id="6a641-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="6a641-108">**Not:** Oturum açma veya etkinleştirme sorunlarını çözmek için modern kimlik doğrulaması (ADAL) veya web hesabı yönetimi (WAM) devre dışı  **bırakılmayabilir**.</span><span class="sxs-lookup"><span data-stu-id="6a641-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="6a641-109">Office 2013 kullanılarak Microsoft 365 'e bağlanırken hatalar oluşursa, Office istemcisi için [modern kimlik doğrulamasını etkinleştirmenizi](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  sağlayın.</span><span class="sxs-lookup"><span data-stu-id="6a641-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="6a641-110">Belirli sorun giderme eylemleri için bkz:</span><span class="sxs-lookup"><span data-stu-id="6a641-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="6a641-111">Windows 10'da, Office 2016 derleme 16.0.7967'ye güncelleştirmeden sonra oturum açmada bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="6a641-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="6a641-112">Office 365, Azure veya Intune gibi kuruluş hesabınızda oturum açamazsınız</span><span class="sxs-lookup"><span data-stu-id="6a641-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="6a641-113">Office 365, Azure veya Intune 'da oturum açmayan tarayıcı olmayan uygulamalarda nasıl sorun giderilir</span><span class="sxs-lookup"><span data-stu-id="6a641-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="6a641-114">Office 'te sürekli kimlik bilgileri isteniyor</span><span class="sxs-lookup"><span data-stu-id="6a641-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)