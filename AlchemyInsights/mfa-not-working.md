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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250185"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="45785-102">MFA ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="45785-102">Issues with MFA</span></span>
<span data-ttu-id="45785-103">Birkaç þey kullanıcılar oturum açılamaz, çok faktörlü kimlik doğrulama (MFA) kullanarak denetlemek için vardır.</span><span class="sxs-lookup"><span data-stu-id="45785-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="45785-104">Etkilenen kullanıcının Azure Active Directory Portal engellenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="45785-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="45785-105">Bu durumda, kimlik doğrulama için otomatik olarak belirli bir kullanıcı engellenir çalışır.</span><span class="sxs-lookup"><span data-stu-id="45785-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="45785-106">Lütfen bunları engelini kaldırmak için bu makalede anlatılan adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="45785-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="45785-107">Kullanıcı engellemesinin kaldırılması gelmedi yardımcı veya kullanıcı bloke MFA kullanıcı için sıfırlamak deneyin ve kaydolma işlemi boyunca tekrar gidecek.</span><span class="sxs-lookup"><span data-stu-id="45785-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="45785-108">Lütfen bu makaledeki adımları izleyin.</span><span class="sxs-lookup"><span data-stu-id="45785-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="45785-109">Bu, etkin MFA ve kullanıcılarınızın Outlook, Skype gibi tarayıcılar olmayan istemciler için oturum açamıyor ilk kez ise, belki de ADAL (Active Directory kimlik doğrulama Kütüphanesi) O365 aboneliğiniz etkin değil.</span><span class="sxs-lookup"><span data-stu-id="45785-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="45785-110">Bu durumda, çevrimiçi Exchange Powershell için bağlanmak ve bu cmdlet'i çalıştırmak gerekir:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="45785-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>