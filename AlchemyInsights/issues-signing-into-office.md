---
title: Office uygulamalarında oturum açma sorunları
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763021"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="39d4b-102">Office uygulamalarında oturum açma sorunları</span><span class="sxs-lookup"><span data-stu-id="39d4b-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="39d4b-103">Office uygulamalarıyla ilgili oturum açma sorunlarını gidermek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="39d4b-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="39d4b-104">Windows Ayarları > **Access çalışmasını veya okul'u**kullanarak etkilenen hesap dışındaki tüm iş hesaplarını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="39d4b-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="39d4b-105">Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)</span><span class="sxs-lookup"><span data-stu-id="39d4b-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="39d4b-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="39d4b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="39d4b-107">(Ör. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="39d4b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="39d4b-108">Office uygulaması açın, **Dosya** > **Hesabı** > **Oturum Aç'ı**seçin. Ardından geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="39d4b-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="39d4b-109">Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="39d4b-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="39d4b-110">Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="39d4b-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="39d4b-111">Office 2013'u kullanarak Microsoft 365'e bağlanırken hatalar oluşursa, Office istemcisi için modern kimlik doğrulamasını etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="39d4b-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="39d4b-112">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="39d4b-112">For more information, see:</span></span>
- [<span data-ttu-id="39d4b-113">Microsoft 365, Azure veya Intune'da oturum açamam</span><span class="sxs-lookup"><span data-stu-id="39d4b-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="39d4b-114">Office 2016'ya güncelleştirmeden sonra oturum açma sorunları Windows 10'da 16.0.7967 oluşturma</span><span class="sxs-lookup"><span data-stu-id="39d4b-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="39d4b-115">Office'te "Üzgünüz, kuruluşunuzdaki başka bir hesap zaten bu bilgisayarda oturum açmış"</span><span class="sxs-lookup"><span data-stu-id="39d4b-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="39d4b-116">ADFS kullanırken Office modern kimlik doğrulamasıyla ilgili oturum açma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="39d4b-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)