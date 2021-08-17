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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055574"
---
# <a name="how-to-enable-hosted-voicemail"></a>Barındırılan Sesli Mesaj nasıl etkinleştirilen

Sesli Mesajı etkinleştirmek için **HostedVoicemail** seçeneği Sesli Mesaj olarak $true.

Remote PowerShell (RPS) kullanan **kullanıcıda HostedVoicemail** özelliği.

RPS'ye bağlanma hakkında daha fazla bilgi için bkz. Microsoft Teams RPS'ye bağlanma hakkında daha fazla bilgi için [PowerShell'e](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) Genel Bakış.

1. Yönetici Teams, diğer kullanıcılar için Remote PowerShell'de oturum Teams.
1. Teams Admin PowerShell isteminden **set-csuser user@contoso.com -HostedVoiceMail $true** çalıştırarak söz konusu kullanıcının sip uri'si olabilir.

> [!NOTE]
> İlkelerde yapılan değişikliklerin çoğaltılması 24 saat kadar sürebilir.