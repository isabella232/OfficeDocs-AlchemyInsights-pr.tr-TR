---
title: Özel kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005458"
---
# <a name="private-channels-in-microsoft-teams"></a>Microsoft Teams'deki özel kanallar

Özel kanallar Microsoft Teams'de yeni bir özelliktir. Özel kanalların standart kanallardan dönüştürülemeyeceğini veya bunun tersi olduğunu unutmayın.

[Özel kanal oluşturma ve üyelik ve](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) özel kanal [SharePoint siteleri](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)hakkındaki bilgiler gibi özel kanallar hakkında ayrıntılı bilgi için Microsoft [Teams'deki Özel kanallara](https://docs.microsoft.com/MicrosoftTeams/private-channels)bakın. 

**Not:** Özel kanal iletilerinin bekletme yapılandırması henüz desteklenmediğinden, bekletme ilkeleri etkinleştirilmiş kiracılar varsayılan olarak özel kanalları etkinleştirmez. Takımlar yönetici merkezinde özel kanallar etkinleştirilebilir. Ayrıca, özel kanal iletilerinin bekletme desteklenmezken, özel kanallarda paylaşılan dosyaların tutulmasının desteklenir.

**Yeni bir takım sahibine mi ihtiyacınız var?**

Özel kanal sahibiniz ayrılırsa, Teams Powershell aracılığıyla yeni bir takım sahibi ekleyebilirsiniz.


- Teams Powershell'i kurmak için [buraya](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) gidin.

İşte ihtiyacınız olacak cmdlet:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Teams Powershell hakkında daha fazla bilgi için [Bkz. Teams PowerShell Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)
