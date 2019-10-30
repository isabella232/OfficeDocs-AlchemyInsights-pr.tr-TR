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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768857"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA ile ilgili sorunlar
Kullanıcıların çok faktörlü kimlik doğrulaması (MFA) kullanarak oturum açıp açmamalarını kontrol etmek için birkaç şey vardır

1. Etkilenen kullanıcı Azure Etkin Dizin Portalı'nda engellenebilir. Bu durumda, söz konusu kullanıcı için kimlik doğrulama denemeleri otomatik olarak reddedilir. [Lütfen engellerini kaldırmak için bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kullanıcının engelini kaldırmak yardımcı olmadıysa veya kullanıcı engellenmiyorsa, kullanıcı için MFA'yı sıfırlamayı deneyebilirsiniz ve bu işlem yeniden kayıt işleminden geçer. [Lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

MFA'yı ilk kez etkinleştirdiyseniz ve kullanıcılarınız Outlook, Skype, vb. gibi tarayıcı olmayan istemcilere giriş yapamıyorsa, Belki De ADAL (Active Directory Authentication Library) O365 aboneliğinizde etkinleştirilmez. Bu durumda Exchange Online Powershell'e bağlanmanız ve bu cmdlet'i çalıştırmanız gerekir:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*