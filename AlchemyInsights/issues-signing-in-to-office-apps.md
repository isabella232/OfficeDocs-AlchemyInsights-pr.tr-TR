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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833095"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="a63f0-102">Microsoft 365 uygulamalarını düzeltme "Üzgünüz, kuruluşun başka bir hesabı zaten oturum açık" iletisi</span><span class="sxs-lookup"><span data-stu-id="a63f0-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="a63f0-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="a63f0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="a63f0-104">Etkilenen hesap hariç tüm iş hesaplarını, Windows Ayarları'> **Access iş veya okul hesabı ile kaldırın.**</span><span class="sxs-lookup"><span data-stu-id="a63f0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="a63f0-105">Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.</span><span class="sxs-lookup"><span data-stu-id="a63f0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a63f0-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti.</span><span class="sxs-lookup"><span data-stu-id="a63f0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a63f0-107">(Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a63f0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a63f0-108">Bir Office uygulamasını açın, Dosya **Hesabı Oturum**  >  **Açma'yi**  >  **seçin.** Ardından, geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="a63f0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="a63f0-109">Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a63f0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a63f0-110">Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="a63f0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="a63f0-111">Daha fazla bilgi için [Office'te "Üzgünüz,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)bu bilgisayarda kuruluştan başka bir hesap oturum alandı" bilgilerine bakın.</span><span class="sxs-lookup"><span data-stu-id="a63f0-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>