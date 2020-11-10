---
title: Gıfın ekip konuşmalarını kullanma
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982574"
---
# <a name="using-giphys-in-teams-conversations"></a>Gıfın ekip konuşmalarını kullanma

Ekipler sohbetinde gifiziksel erişim varsayılan olarak etkinleştirilmiştir. Yönetici olarak, [bir mesajlaşma ilkesi ayarlayarak](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ve **gifin konuşmaların** **Açık** olduğundan emin olmak için gıas kullanıcıları tarafından kullanılabilir olup olmadığını denetleyebilirsiniz.

Gelen GIF 'Ler ekip konuşmalarında beklendiği gibi çalışmıyorsa aşağıdakileri doğrulayın:

[Mesajlaşma ilkesi](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) , gifiziksel. PowerShell cmdlet 'lerini kullanarak doğrulamak için:

- [PowerShell Ile takımları yönetebildiğinizi](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)doğrulayın.
- [Get-CsTeamsMessagingPolicy-Identity genel](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) PowerShell komutunu çalıştırarak, **Allowgiphy** 'ın **true** olarak ayarlandığını doğrulayın.
- **Allowgiphy** **yanlış** olarak ayarlanmışsa, aşağıdaki PowerShell komut [kümesi-CsTeamsMessagingPolicy-Identity Global-allowgıphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Giphy URL 'ye erişime izin vermek için [Isteğe bağlı bağlantılı deneyimlerin](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) etkinleştirilmesi gerekir.

> [!NOTE]
> Kiracınız için yapılandırılmış birden fazla ekip mesajlaşma ilkeniz varsa, etkilenen kullanıcıya atanan ilkenin kimliğini [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | PowerShell komutuyla belirleyebilirsiniz. <user@domain.com> TeamsMessagingPolicy öğesini seçin.
