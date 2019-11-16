---
title: MFA ile ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768857"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="c9b06-102">Azure MFA ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="c9b06-102">Issues with Azure MFA</span></span>
<span data-ttu-id="c9b06-103">Kullanıcıların çok faktörlü kimlik doğrulaması (MFA) kullanarak oturum açıp açmamalarını kontrol etmek için birkaç şey vardır</span><span class="sxs-lookup"><span data-stu-id="c9b06-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="c9b06-104">Etkilenen kullanıcı Azure Etkin Dizin Portalı'nda engellenebilir.</span><span class="sxs-lookup"><span data-stu-id="c9b06-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="c9b06-105">Bu durumda, söz konusu kullanıcı için kimlik doğrulama denemeleri otomatik olarak reddedilir.</span><span class="sxs-lookup"><span data-stu-id="c9b06-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="c9b06-106">Lütfen engellerini kaldırmak için bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="c9b06-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="c9b06-107">Kullanıcının engelini kaldırmak yardımcı olmadıysa veya kullanıcı engellenmiyorsa, kullanıcı için MFA'yı sıfırlamayı deneyebilirsiniz ve bu işlem yeniden kayıt işleminden geçer.</span><span class="sxs-lookup"><span data-stu-id="c9b06-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="c9b06-108">Lütfen bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="c9b06-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="c9b06-109">MFA'yı ilk kez etkinleştirdiyseniz ve kullanıcılarınız Outlook, Skype, vb. gibi tarayıcı olmayan istemcilere giriş yapamıyorsa, Belki De ADAL (Active Directory Authentication Library) O365 aboneliğinizde etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="c9b06-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="c9b06-110">Bu durumda Exchange Online Powershell'e bağlanmanız ve bu cmdlet'i çalıştırmanız gerekir:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="c9b06-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>