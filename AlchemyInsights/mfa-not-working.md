---
title: MFA ile ilgili sorunlar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810504"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="1d98d-102">Azure MFA ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="1d98d-102">Issues with Azure MFA</span></span>
<span data-ttu-id="1d98d-103">Kullanıcıların Multi-Factor Authentication (MFA) kullanarak oturum açamalarını denetlemenin birkaç yöntemi vardır</span><span class="sxs-lookup"><span data-stu-id="1d98d-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="1d98d-104">Etkilenen kullanıcı Azure Active Directory Portalı'ta engellenebilir.</span><span class="sxs-lookup"><span data-stu-id="1d98d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="1d98d-105">Böyle bir durumda, belirli bir kullanıcı için kimlik doğrulaması girişimleri otomatik olarak reddedilir.</span><span class="sxs-lookup"><span data-stu-id="1d98d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="1d98d-106">Engelini kaldırmak için lütfen bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="1d98d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="1d98d-107">Kullanıcının engellemesini kaldırmak işe yaramamışsa veya kullanıcı engellenmişse, kullanıcı için MFA'yı sıfırlamayı deneyebilir ve kullanıcı kayıt işlemini tamamlar.</span><span class="sxs-lookup"><span data-stu-id="1d98d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="1d98d-108">Lütfen bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="1d98d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="1d98d-109">MFA'ı ilk kez etkinleştiriyorsanız ve kullanıcılarınız Outlook, Skype gibi tarayıcı olmayan istemcilerinde oturum açamıyorsa, belki de O365 aboneliğiniz üzerinde ADAL (Active Directory Authentication Library) etkin değildir.</span><span class="sxs-lookup"><span data-stu-id="1d98d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="1d98d-110">Bu durumda Exchange Online Powershell'e bağlanmanız ve Şu cmdlet'i çalıştırmanız gerekir:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="1d98d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>