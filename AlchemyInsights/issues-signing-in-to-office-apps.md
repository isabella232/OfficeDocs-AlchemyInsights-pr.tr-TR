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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938373"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="eb908-102">Office apps "Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanmış" iletisini çözme</span><span class="sxs-lookup"><span data-stu-id="eb908-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="eb908-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="eb908-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="eb908-104">Windows ayarları > **erişim iş veya Okul**kullanarak etkilenen hesabı dışındaki tüm çalışma hesapları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="eb908-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="eb908-105">Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="eb908-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="eb908-106">**Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti.</span><span class="sxs-lookup"><span data-stu-id="eb908-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="eb908-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="eb908-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="eb908-108">Bir Office uygulamasını açın, **Dosya** > **Hesap** > **Oturumu Kapat**. Sonra geçerli bir lisansa bir kullanıcı hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="eb908-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="eb908-109">Ayrıntılı bilgi için bkz: [Office hesapları](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="eb908-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="eb908-110">Mac için bkz: [Mac app için bir Office 2016'da oturum açamıyorsunuz](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="eb908-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="eb908-111">Daha fazla bilgi için bkz: ["Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanan bu bilgisayar üzerinde" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="eb908-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>