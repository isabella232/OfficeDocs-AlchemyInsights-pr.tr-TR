---
title: Office uygulamaları için oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938374"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="bf5c0-102">Office uygulamaları için oturum açma sorunları</span><span class="sxs-lookup"><span data-stu-id="bf5c0-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="bf5c0-103">Office uygulamaları ile oturum açma sorunlarını düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="bf5c0-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="bf5c0-104">Windows ayarları > **erişim iş veya Okul**kullanarak etkilenen hesabı dışındaki tüm çalışma hesapları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="bf5c0-105">Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="bf5c0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bf5c0-106">**Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bf5c0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bf5c0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="bf5c0-108">Bir Office uygulamasını açın, **Dosya** > **Hesap** > **Oturumu Kapat**. Sonra geçerli bir lisansa bir kullanıcı hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="bf5c0-109">Ayrıntılı bilgi için bkz: [Office hesapları](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="bf5c0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="bf5c0-110">Mac için bkz: [Mac app için bir Office 2016'da oturum açamıyorsunuz](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="bf5c0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="bf5c0-111">Hatalar oluşursa, Office kullanarak Office 2013 365 bağlanırken, Office istemcisi için modern kimlik doğrulamasını etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="bf5c0-112">Daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-112">For more information, see:</span></span>
- [<span data-ttu-id="bf5c0-113">Office 365, Azure veya Intune oturum açamıyorum</span><span class="sxs-lookup"><span data-stu-id="bf5c0-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="bf5c0-114">Oturum açmak için Office 2016 güncelleştirmeden sonra bağlantı sorunları 16.0.7967 Windows 10 üzerinde oluşturun.</span><span class="sxs-lookup"><span data-stu-id="bf5c0-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="bf5c0-115">"Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanan bu bilgisayar üzerinde" Office</span><span class="sxs-lookup"><span data-stu-id="bf5c0-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="bf5c0-116">ADFS kullandığınızda Office modern kimlik doğrulamasıyla oturum sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="bf5c0-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)