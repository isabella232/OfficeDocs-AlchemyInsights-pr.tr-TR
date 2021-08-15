---
title: Farklı bağlantı noktaları erişim sorunları için tanılama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030922"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Farklı bağlantı noktaları erişim sorunları için tanılama

Farklı bağlantı noktası erişim sorunlarını çözmek için aşağıdaki adımları izleyin:

1. Sanal makinesi (VM) portaldan durdurun/deneyin, VM'yi yeniden başlatın ve yeniden test edin. 
2. Sanal makinenizin ağ ayarlarını kontrol edin ve trafiği engelleyen Ağ Güvenlik Grupları (NSG) olup olmadığını kontrol edin. Ayrıca, Ağ [Watcher'ın IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) akış doğrulama aracını kullanarak trafiği engelleyen NSG'ler, User-Defined Yönlendirmeleri (UDR) trafiğinizi yeniden şirket içi bir cihaza ('Varsayılan Rota' 0.0.0.0/0) veya bir ağ cihazına yönlendirebilirsiniz.
Yukarıdaki adımları denemenin ardından sorun olmaya devam ediyorsanız, lütfen VM adını ve daha fazla tanı için posta göndermeye çalıştığınız TCP bağlantı noktasını girin.

**Önerilen Belgeler**

[Bağlantı noktası 25 üzerinden giden e-posta gönderme sınırlamaları ve önerileri](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)