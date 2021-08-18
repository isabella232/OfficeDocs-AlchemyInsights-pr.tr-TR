---
title: Barındırılan Sesli Mesaj nasıl etkinleştirilen
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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318668"
---
# <a name="how-to-enable-hosted-voicemail"></a>Barındırılan Sesli Mesaj nasıl etkinleştirilen

Sesli Mesajı etkinleştirmek için **HostedVoicemail** seçeneği Sesli Mesaj olarak $true.

Remote PowerShell (RPS) kullanan **kullanıcıda HostedVoicemail** özelliği.

RPS'ye bağlanma hakkında daha fazla bilgi için bkz. Microsoft Teams RPS'ye bağlanma hakkında daha fazla bilgi için [PowerShell'e](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) Genel Bakış.

1. Sistem Teams, diğer kullanıcılar için Remote PowerShell'de oturum Teams.
1. Teams Admin PowerShell isteminden **set-csuser user@contoso.com -HostedVoiceMail $true'i** çalıştırarak söz konusu kullanıcının sip uri'si olabilir.

**Not:** İlkelerde yapılan değişikliklerin çoğaltılması 24 saat kadar sürebilir.