---
title: Konuşmalarda Giphys Teams kullanma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323540"
---
# <a name="using-giphys-in-teams-conversations"></a>Konuşmalarda Giphys Teams kullanma

Sohbette Giphys Teams varsayılan olarak etkindir. Yönetici olarak, bir ileti ilkesi ayarp Görüşmelerde [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy kullanımı ayarının Açık olduğu hakkında bilgi sağlayarak, kullanıcıları **Giphys'in kullanııp kullanamaya olduğunu** kontrol **etmek için kullanabilirsiniz.**

Bu konuşmalarda GIF'ler beklendiği gibi Teams, şunları doğrulayın:

[Giphys'e](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) izin vermek için ileti ilkesi gerekir. PowerShell cmdlet'lerini kullanarak doğrulamak için:

- [Teams'i PowerShell ile yönet'inizi doğrulayın.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) PowerShell komutunu çalıştırın ve **AllowGiphy'in** TRUE olarak ayar olduğunu **doğrulayın.**
- **AllowGiphy** **YANLIŞ** olarak ayarlanırsa, aşağıdaki PowerShell komutunu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Giphy URL'sine](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) erişim izni vermek için isteğe bağlı Bağlı Deneyimlerin etkinleştirilmesi gerekir.

**Not:** Kiracınız için birden Teams Mesajlaşma ilkeleri yapılandırılmışsa, etki altında olan kullanıcıya atanan ilkenin kimliğini [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) PowerShell komutuyla <user@domain.com> | TeamsMessagingPolicy seçeneğini seçin.
