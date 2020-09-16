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
# <a name="issues-with-azure-mfa"></a>Azure MFA 'daki sorunlar
Kullanıcıların Multi-Factor Authentication (MFA) kullanarak oturum açıp açamayacağınızı denetlemek için birkaç şey vardır

1. Etkilenen Kullanıcı Azure Active Directory portalında engellenmiş olabilir. Bu durumda, söz konusu kullanıcının kimlik doğrulama denemeleri otomatik olarak reddedilir. [Bu makaledeki adımları izleyerek bunları kaldırın.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kullanıcının engellenmesini kaldırma konusunda yardım yoksa veya Kullanıcı engellenmediyse, Kullanıcı için MFA sıfırlamayı deneyebilirsiniz ve kayıt işlemini yeniden ilerler. [Lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Bu, MFA 'yi ilk kez etkinleştirdiyseniz, kullanıcılarınız Outlook, Skype gibi tarayıcılarda olmayan istemcilerde oturum açmayabilir, ancak O365 aboneliğinizde bir ADAL (Active Directory kimlik doğrulama kitaplığı) etkinleştirilmez. Bu durumda, Exchange Online PowerShell 'e bağlanmanız ve şu cmdlet 'i çalıştırmanız gerekir:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*