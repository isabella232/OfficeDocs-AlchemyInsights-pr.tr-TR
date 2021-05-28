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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696978"
---
# <a name="11-call-recording"></a>Bire bir arama kaydı

Bir **aramada** Kaydı Başlat düğmesi gri görüntüye sahipse, etkiyi alan kullanıcının ilke ayarlarını değiştirmeniz gerekir.   

31 Mayıs 2021'den başlayarak, *AllowCloudRecordingForCalls* için yeni bir Çağrı Teams zorlamaya başlayacağız. Bu değişiklikten önce, 1:1 arama kaydı Toplantı İlkesi'ne göre *AllowCloudRecording* Teams denetlenir. Bu değişiklik İleti Merkezi gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1 Arama kaydı ilkesi giriş.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   arama ilkesi seçeneği varsayılan olarak **$False** olarak ayarlanır. Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işleme gerek yok.  

Bire bir aramalarda tüm kullanıcılar için arama kaydını etkinleştirmek üzere Teams PowerShell'i kullanarak aşağıdaki cmdlet'i çalıştırın: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternatif olarak, yeni bir ilke oluşturabilir ve **-AllowCloudRecordingForCalls** $true bu ilkeyi ayarlayarak kullanıcılarınıza atabilirsiniz.  

Daha fazla bilgi için [bkz. 1:1 Arama Kaydı İlkesi Denetimleri (Neredeyse!) Burada.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
