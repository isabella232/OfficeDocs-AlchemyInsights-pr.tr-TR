---
title: Konuşmalarda Giphy'Teams kullanma
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104328"
---
# <a name="using-giphys-in-teams-conversations"></a>Konuşmalarda Giphy'Teams kullanma

Sohbette Giphys Teams varsayılan olarak etkindir. Yönetici olarak, bir ileti ilkesi ayarp Görüşmelerde [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy kullanımı ayarının Açık olduğu hakkında bilgi sağlayarak, kullanıcıları **Giphys'in kullanııp kullanamaya olduğunu** kontrol **etmek için kullanabilirsiniz.**

Bu görüşmelerde GIF'ler beklendiği gibi Teams, şunları doğrulayın:

[Giphys'e](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) izin vermek için ileti ilkesi gerekir. PowerShell cmdlet'lerini kullanarak doğrulamak için:

- [Teams'i PowerShell ile yönetenizi doğrulayın.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) PowerShell komutunu çalıştırın ve **AllowGiphy'in** TRUE olarak ayar olduğunu **doğrulayın.**
- **AllowGiphy** **YANLIŞ** olarak ayarlanırsa, aşağıdaki PowerShell komutunu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Giphy URL'sine](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) erişim izni vermek için isteğe bağlı Bağlı Deneyimlerin etkinleştirilmesi gerekir.

> [!NOTE]
> Kiracınız için yapılandırılmış birden Teams mesajlaşma ilkeleriniz varsa, [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) PowerShell komutuyla, etki altında olan kullanıcıya atanan ilkenin kimliğini <user@domain.com> | TeamsMessagingPolicy seçeneğini seçin.
