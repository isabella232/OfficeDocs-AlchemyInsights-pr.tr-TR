---
title: MFA ile ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755151"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="2d7f5-102">Azure MFA 'daki sorunlar</span><span class="sxs-lookup"><span data-stu-id="2d7f5-102">Issues with Azure MFA</span></span>
<span data-ttu-id="2d7f5-103">Kullanıcıların Multi-Factor Authentication (MFA) kullanarak oturum açıp açamayacağınızı denetlemek için birkaç şey vardır</span><span class="sxs-lookup"><span data-stu-id="2d7f5-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2d7f5-104">Etkilenen Kullanıcı Azure Active Directory portalında engellenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2d7f5-105">Bu durumda, söz konusu kullanıcının kimlik doğrulama denemeleri otomatik olarak reddedilir.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2d7f5-106">Bu makaledeki adımları izleyerek bunları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2d7f5-107">Kullanıcının engellenmesini kaldırma konusunda yardım yoksa veya Kullanıcı engellenmediyse, Kullanıcı için MFA sıfırlamayı deneyebilirsiniz ve kayıt işlemini yeniden ilerler.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2d7f5-108">Lütfen bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2d7f5-109">Bu, MFA 'yi ilk kez etkinleştirdiyseniz, kullanıcılarınız Outlook, Skype gibi tarayıcılarda olmayan istemcilerde oturum açmayabilir, ancak O365 aboneliğinizde bir ADAL (Active Directory kimlik doğrulama kitaplığı) etkinleştirilmez.</span><span class="sxs-lookup"><span data-stu-id="2d7f5-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2d7f5-110">Bu durumda, Exchange Online PowerShell 'e bağlanmanız ve şu cmdlet 'i çalıştırmanız gerekir:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="2d7f5-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>