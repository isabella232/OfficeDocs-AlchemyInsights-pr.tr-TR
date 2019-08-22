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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545205"
---
# <a name="issues-with-mfa"></a>MFA ile ilgili sorunlar
Birkaç þey kullanıcılar oturum açılamaz, çok faktörlü kimlik doğrulama (MFA) kullanarak denetlemek için vardır.

1. Etkilenen kullanıcının Azure Active Directory Portal engellenmiş olabilir. Bu durumda, kimlik doğrulama için otomatik olarak belirli bir kullanıcı engellenir çalışır. [Lütfen bunları engelini kaldırmak için bu makalede anlatılan adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Kullanıcı engellemesinin kaldırılması gelmedi yardımcı veya kullanıcı bloke MFA kullanıcı için sıfırlamak deneyin ve kaydolma işlemi boyunca tekrar gidecek. [Lütfen bu makaledeki adımları izleyin.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Bu, etkin MFA ve kullanıcılarınızın Outlook, Skype gibi tarayıcılar olmayan istemciler için oturum açamıyor ilk kez ise, belki de ADAL (Active Directory kimlik doğrulama Kütüphanesi) O365 aboneliğiniz etkin değil. Bu durumda, çevrimiçi Exchange Powershell için bağlanmak ve bu cmdlet'i çalıştırmak gerekir:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*