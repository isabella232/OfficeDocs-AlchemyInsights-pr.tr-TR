---
title: NDI teknolojisini açma
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935196"
---
# <a name="turn-on-ndi-technology"></a>NDI teknolojisini açma

NDI teknolojisi bir kullanıcı için iki adımın açık olması gerekir:

1. Kiracı yöneticisinin CsTeamsMeetingPolicy'de 'AllowNDIStreaming' özelliğini etkinleştirmesi gerekir.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Bu değişiklik doldurulduğunda, son kullanıcının Ayarlar ve İzinler'den ® istemci için NDI> **açması gerekir.**

Daha fazla bilgi için Microsoft [Teams'de NDI teknolojisini kullanma.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
