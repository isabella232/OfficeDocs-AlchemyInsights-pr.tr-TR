---
title: Bire bir arama kaydı
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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314404"
---
# <a name="11-call-recording"></a>Bire bir arama kaydı

Bir **aramada** Kaydı Başlat düğmesi gri görüntüye sahipse, etkiyi alan kullanıcının ilke ayarlarını değiştirmeniz gerekir. İlke ayarını kontrol etmek için, yukarıdaki **Diag: 1:1** Arama Kaydı yazarak etki Teams Tanılama'yı çalıştırın.     

31 Mayıs 2021'den başlayarak, Yeni bir Arama İlkesi *AllowCloudRecordingForCalls Teams zorlamaya başlayacağız.* Bu değişiklikten önce, 1:1 arama kaydı Toplantı İlkesi'ne göre *AllowCloudRecording* Teams denetlenir. Bu değişiklik İleti Merkezi gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1 Arama kaydı ilkesi giriş.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   arama ilkesi seçeneği varsayılan olarak **$False** olarak ayarlanır. Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işleme gerek yok.  

Bire bir aramalarda tüm kullanıcılarda arama kaydını etkinleştirmek için Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) kullanarak aşağıdaki cmdlet'i çalıştırın: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatif olarak, yeni bir ilke oluşturabilir ve **-AllowCloudRecordingForCalls** $true ilkeyi ayarlayarak kullanıcılarınıza atabilirsiniz.  

Daha fazla bilgi için [bkz. 1:1 Arama Kaydı İlkesi Denetimleri (Neredeyse!) Burada.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
