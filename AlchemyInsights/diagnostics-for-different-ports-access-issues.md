---
title: Farklı bağlantı noktalarına erişim sorunları için tanılama
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036805"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Farklı bağlantı noktalarına erişim sorunları için tanılama

Farklı bağlantı noktası erişim sorunlarını çözmek için aşağıdaki adımları uygulayın:

1. Sanal makineyi (VM) portaldan durdurun/yeniden başlatın, VM'yi yeniden başlatın ve yeniden test edin. 
2. Trafiği engelleyen Ağ Güvenlik Grupları (NSG) olup olmadığını belirlemek için VM'nizin ağ ayarlarını kontrol edin. Ayrıca, Ağ [](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) İzleme aracını kullanarak trafiği engelleyen NSG'leri, trafiğinizi yeniden şirket içi yönlendirmeye ('Varsayılan Rota' 0.0.0.0/0) User-Defined Yönlendirmeleri'ne veya bir ağ cihazına yönlendirebilirsiniz.
Yukarıdaki adımları denemenin ardından sorun olmaya devam ediyorsanız, lütfen daha fazla tanı için posta göndermeye çalıştığınız VM adını ve TCP bağlantı noktasını girin.

**Önerilen Belgeler**

[Bağlantı noktası 25 üzerinden giden e-posta göndermeye ilişkin sınırlamalar ve öneriler](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)