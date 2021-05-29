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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702110"
---
# <a name="11-call-recording"></a>Bire bir arama kaydı

Bir **aramada** Kaydı Başlat düğmesi gri görüntüye sahipse, etkiyi alan kullanıcının ilke ayarlarını değiştirmeniz gerekir. İlke ayarını kontrol etmek için, yukarıdaki **Diag: 1:1** Arama Kaydı yazın ve etki Teams Tanılama'yı çalıştırın.     

31 Mayıs 2021'den başlayarak, *AllowCloudRecordingForCalls* için yeni bir Çağrı Teams zorlamaya başlayacağız. Bu değişiklikten önce, 1:1 arama kaydı Toplantı İlkesi'ne göre *AllowCloudRecording* Teams denetlenir. Bu değişiklik İleti Merkezi gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1 Arama kaydı ilkesi giriş.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   arama ilkesi seçeneği varsayılan olarak **$False** olarak ayarlanır. Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işleme gerek yok.  

Bire bir aramalarda tüm kullanıcılarda arama kaydını etkinleştirmek için [Teams PowerShell](/microsoftteams/teams-powershell-install) kullanarak aşağıdaki cmdlet'i çalıştırın: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatif olarak, yeni bir ilke oluşturabilir ve **-AllowCloudRecordingForCalls** $true bu ilkeyi ayarlayarak kullanıcılarınıza atabilirsiniz.  

Daha fazla bilgi için [bkz. 1:1 Arama Kaydı İlkesi Denetimleri (Neredeyse!) Burada.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
