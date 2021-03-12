---
title: 1:1 arama kaydı
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733869"
---
# <a name="11-call-recording"></a>1:1 arama kaydı

Yöneticilerin, kullanıcıların 1:1 arama kaydetmelerine izin vermeye devam etmek için hemen harekete geçleri gerekir.
 
12 Nisan 2021'den itibaren, yeni bir Teams Arama İlkesi *seçeneği AllowCloudRecordingForCalls'u zorlamaya başlayacağız.* 

Şu anda 1:1 arama kaydı özellikleri, Teams Toplantı *İlkeleri'nin AllowCloudRecording* seçeneği tarafından denetlenmektedir. Kullanıcılarının Teams Toplantıları kaydetmesine izin veriliyorsa, bire bir aramaları da kaydedebilirsiniz.

Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işlem yapmaya gerek yok. *AllowCloudRecordingForCalls* arama ilkesi seçeneği varsayılan $False kullanılabilir.

Bu değişiklik, şu İleti Merkezi Gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Arama kaydı ilkesine giriş Teams Arama İlkesi Seçeneğini ayarlamak için [Teams PowerShell'i kullanasınız.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Bire bir aramalarda** arama kaydını etkinleştirmek için: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Bire bir aramalarda** arama kaydını devre dışı bırakmak için: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

