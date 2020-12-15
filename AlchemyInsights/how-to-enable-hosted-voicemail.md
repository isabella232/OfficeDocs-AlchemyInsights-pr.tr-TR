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
# <a name="how-to-enable-hosted-voicemail"></a>Barındırılan sesli mesajı etkinleştirme

Sesli mesajı etkinleştirmek için, **Hostedsesli mesaj** $true olarak ayarlanmalıdır.

Kullanıcıya uzak PowerShell (RPS) kullanarak **Hostedsesli mesaj** özelliği.

RPS 'ye bağlanma hakkında daha fazla bilgi için, RPS 'ye bağlanma hakkında daha fazla bilgi için [Microsoft ekipleri PowerShell 'e genel bakış](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) konusuna bakın.

1. Ekip Yöneticisi ekip için uzak PowerShell 'e oturum açmış olmalıdır.
1. PowerShell 'in söz konusu Kullanıcı olduğu PowerShell URI 'si olan **Set-CsUser user@contoso.com-Hostedsesli mesaj $true** ,

> [!NOTE]
> İlkelerde yapılan değişikliklerin çoğaltılması 24 saate kadar sürebilir.