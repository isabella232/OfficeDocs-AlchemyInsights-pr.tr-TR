---
title: Microsoft 365 uygulamalarında oturum açma sorunları
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579957"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="f04c4-102">Microsoft 365 uygulamalarını düzeltme "Üzgünüz, kuruluşunuzdaki başka bir hesap zaten oturum açmış durumda" iletisi</span><span class="sxs-lookup"><span data-stu-id="f04c4-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="f04c4-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="f04c4-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="f04c4-104">Windows Ayarları > **Access çalışmasını veya okul'u**kullanarak etkilenen hesap dışındaki tüm iş hesaplarını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="f04c4-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="f04c4-105">Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)</span><span class="sxs-lookup"><span data-stu-id="f04c4-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f04c4-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="f04c4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f04c4-107">(Ör. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f04c4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="f04c4-108">Office uygulaması açın, **File**  >  **Dosya Hesabı**Oturum  >  **Aç'ı**seçin. Ardından geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f04c4-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="f04c4-109">Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="f04c4-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="f04c4-110">Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="f04c4-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="f04c4-111">Daha fazla bilgi için [Bkz. "Üzgünüz, kuruluşunuzdan başka bir hesap zaten bu bilgisayarda oturum açmış" Office'te.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="f04c4-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>