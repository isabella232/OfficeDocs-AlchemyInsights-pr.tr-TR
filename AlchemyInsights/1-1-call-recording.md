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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886159"
---
# <a name="11-call-recording"></a>Bire bir arama kaydı

Bir **aramada** Kaydı Başlat düğmesi gri görüntüye sahipse, etkiyi alan kullanıcının ilke ayarlarını değiştirmeniz gerekir. İlke ayarını kontrol etmek için, yukarıdaki **Diag: 1:1** Arama Kaydı yazın ve etki Teams Tanılama'yı çalıştırın.     

31 Mayıs 2021'den başlayarak, *AllowCloudRecordingForCalls* için yeni bir Çağrı Teams zorlamaya başlayacağız. Bu değişiklikten önce, 1:1 arama kaydı Toplantı İlkesi'ne göre *AllowCloudRecording* Teams denetlenir. Bu değişiklik İleti Merkezi gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1 Arama kaydı ilkesi giriş.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   arama ilkesi seçeneği varsayılan olarak **$False** olarak ayarlanır. Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işleme gerek yok.  

Bire bir aramalarda tüm kullanıcılarda arama kaydını etkinleştirmek için [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) kullanarak aşağıdaki cmdlet'i çalıştırın: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatif olarak, yeni bir ilke oluşturabilir ve **-AllowCloudRecordingForCalls** $true ilkeyi ayarlayarak kullanıcılarınıza atabilirsiniz.  

Daha fazla bilgi için [bkz. 1:1 Arama Kaydı İlkesi Denetimleri (Neredeyse!) Burada.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
