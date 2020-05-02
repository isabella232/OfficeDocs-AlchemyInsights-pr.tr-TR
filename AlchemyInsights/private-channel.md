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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="8d1ed-102">Microsoft Teams'deki özel kanallar</span><span class="sxs-lookup"><span data-stu-id="8d1ed-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="8d1ed-103">Özel kanallar Microsoft Teams'de yeni bir özelliktir.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="8d1ed-104">Özel kanalların standart kanallardan dönüştürülemeyeceğini veya bunun tersi olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="8d1ed-105">[Özel kanal oluşturma ve üyelik ve](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) özel kanal [SharePoint siteleri](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)hakkındaki bilgiler gibi özel kanallar hakkında ayrıntılı bilgi için Microsoft [Teams'deki Özel kanallara](https://docs.microsoft.com/MicrosoftTeams/private-channels)bakın.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="8d1ed-106">**Not:** Özel kanal iletilerinin bekletme yapılandırması henüz desteklenmediğinden, bekletme ilkeleri etkinleştirilmiş kiracılar varsayılan olarak özel kanalları etkinleştirmez.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="8d1ed-107">Takımlar yönetici merkezinde özel kanallar etkinleştirilebilir.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="8d1ed-108">Ayrıca, özel kanal iletilerinin bekletme desteklenmezken, özel kanallarda paylaşılan dosyaların tutulmasının desteklenir.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="8d1ed-109">**Yeni bir takım sahibine mi ihtiyacınız var?**</span><span class="sxs-lookup"><span data-stu-id="8d1ed-109">**Need a new team owner?**</span></span>

<span data-ttu-id="8d1ed-110">Özel kanal sahibiniz ayrılırsa, Teams Powershell aracılığıyla yeni bir takım sahibi ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="8d1ed-111">Teams Powershell'i kurmak için [buraya](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) gidin.</span><span class="sxs-lookup"><span data-stu-id="8d1ed-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="8d1ed-112">İşte ihtiyacınız olacak cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8d1ed-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="8d1ed-113">Teams Powershell hakkında daha fazla bilgi için [Bkz. Teams PowerShell Genel Bakış.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="8d1ed-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
