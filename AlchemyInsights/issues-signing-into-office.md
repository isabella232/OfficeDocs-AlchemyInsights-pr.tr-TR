---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836623"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="a82d7-102">Microsoft 365 Uygulamaları'ta oturum açma sorunları</span><span class="sxs-lookup"><span data-stu-id="a82d7-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="a82d7-103">Microsoft 365 uygulamalarıyla oturum açma sorunlarını çözmek için, etkilenen makinede aşağıdaki seçenekleri deneyin:</span><span class="sxs-lookup"><span data-stu-id="a82d7-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="a82d7-104">Windows için [bkz. Yaygın oturum açma sorunlarını çözme önerileri](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="a82d7-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="a82d7-105">Mac için  [bkz. Office Mac 2016 uygulamasında oturum açama](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="a82d7-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="a82d7-106">**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz.</span><span class="sxs-lookup"><span data-stu-id="a82d7-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="a82d7-107">Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="a82d7-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="a82d7-108">**Not:** Oturum açma veya etkinleştirme sorunlarını düzeltmek için Modern Kimlik Doğrulama (ADAL) veya Web Hesabı Yönetimi'ni (WAM) devre **dışı bırakmanız önerilmez.**</span><span class="sxs-lookup"><span data-stu-id="a82d7-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="a82d7-109">Office 2013'ü kullanarak Microsoft 365'e bağlanırken hata oluşursa, Office istemcisi için [modern kimlik doğrulamayı etkinleştirmeyi](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  denetleyin.</span><span class="sxs-lookup"><span data-stu-id="a82d7-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="a82d7-110">Belirli sorun giderme eylemleri için bkz:</span><span class="sxs-lookup"><span data-stu-id="a82d7-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="a82d7-111">Windows 10'da, Office 2016 derleme 16.0.7967'ye güncelleştirmeden sonra oturum açmada bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="a82d7-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="a82d7-112">Office 365, Azure veya Intune gibi kuruluş hesabınızla oturum acasınız</span><span class="sxs-lookup"><span data-stu-id="a82d7-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="a82d7-113">Office 365, Azure veya Intune'da oturum açmayan tarayıcı olmayan uygulamaların sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="a82d7-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="a82d7-114">Office'te tekrar tekrar kimlik bilgileri istendiğinde</span><span class="sxs-lookup"><span data-stu-id="a82d7-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)