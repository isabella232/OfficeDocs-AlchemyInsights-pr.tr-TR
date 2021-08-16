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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098622"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA ile ilgili sorunlar
Kullanıcıların Multi-Factor Authentication (MFA) kullanarak oturum açamalarını denetlemenin birkaç yöntemi vardır

1. Etkilenen kullanıcı Portal'da Azure Active Directory engellenebilir. Böyle bir durumda, belirli bir kullanıcı için kimlik doğrulaması girişimleri otomatik olarak reddedilir. [Engelini kaldırmak için lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kullanıcının engellemesini kaldırmak işe yaramamışsa veya kullanıcı engellenmişse, kullanıcı için MFA'yı sıfırlamayı deneyebilir ve kullanıcı kayıt işlemini tamamlar. [Lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

MFA'ı ilk kez etkinleştiriyorsanız ve kullanıcılarınız Outlook, Skype gibi tarayıcı olmayan istemcilerinde oturum açamıyorsa, belki de ADAL (Active Directory Authentication Library) O365 aboneliğiniz için etkinleştirilmemiş olabilir. Bu durumda, Exchange Online Powershell'e bağlanmanız ve şu cmdlet'i çalıştırmanız gerekir: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*