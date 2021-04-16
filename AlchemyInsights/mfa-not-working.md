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
# <a name="issues-with-azure-mfa"></a>Azure MFA ile ilgili sorunlar
Kullanıcıların Multi-Factor Authentication (MFA) kullanarak oturum açamalarını denetlemenin birkaç yöntemi vardır

1. Etkilenen kullanıcı Azure Active Directory Portalı'ta engellenebilir. Böyle bir durumda, belirli bir kullanıcı için kimlik doğrulaması girişimleri otomatik olarak reddedilir. [Engelini kaldırmak için lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kullanıcının engellemesini kaldırmak işe yaramamışsa veya kullanıcı engellenmişse, kullanıcı için MFA'yı sıfırlamayı deneyebilir ve kullanıcı kayıt işlemini tamamlar. [Lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

MFA'ı ilk kez etkinleştiriyorsanız ve kullanıcılarınız Outlook, Skype gibi tarayıcı olmayan istemcilerinde oturum açamıyorsa, belki de O365 aboneliğiniz üzerinde ADAL (Active Directory Authentication Library) etkin değildir. Bu durumda Exchange Online Powershell'e bağlanmanız ve Şu cmdlet'i çalıştırmanız gerekir:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*