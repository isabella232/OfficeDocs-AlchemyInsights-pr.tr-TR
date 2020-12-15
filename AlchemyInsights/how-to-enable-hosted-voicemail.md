---
title: Barındırılan sesli mesajı etkinleştirme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679162"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="0395f-102">Barındırılan sesli mesajı etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="0395f-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="0395f-103">Sesli mesajı etkinleştirmek için, **Hostedsesli mesaj** $true olarak ayarlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="0395f-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="0395f-104">Kullanıcıya uzak PowerShell (RPS) kullanarak **Hostedsesli mesaj** özelliği.</span><span class="sxs-lookup"><span data-stu-id="0395f-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="0395f-105">RPS 'ye bağlanma hakkında daha fazla bilgi için, RPS 'ye bağlanma hakkında daha fazla bilgi için [Microsoft ekipleri PowerShell 'e genel bakış](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="0395f-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="0395f-106">Ekip Yöneticisi ekip için uzak PowerShell 'e oturum açmış olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="0395f-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="0395f-107">PowerShell 'in söz konusu Kullanıcı olduğu PowerShell URI 'si olan **Set-CsUser user@contoso.com-Hostedsesli mesaj $true** ,</span><span class="sxs-lookup"><span data-stu-id="0395f-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="0395f-108">İlkelerde yapılan değişikliklerin çoğaltılması 24 saate kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="0395f-108">Changes to policies can take up to 24 hours to replicate.</span></span>