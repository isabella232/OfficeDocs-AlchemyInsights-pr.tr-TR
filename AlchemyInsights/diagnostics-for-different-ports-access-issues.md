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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="6e4aa-102">Farklı bağlantı noktalarına erişim sorunları için tanılama</span><span class="sxs-lookup"><span data-stu-id="6e4aa-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="6e4aa-103">Farklı bağlantı noktası erişim sorunlarını çözmek için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="6e4aa-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="6e4aa-104">Sanal makineyi (VM) portaldan durdurun/yeniden başlatın, VM'yi yeniden başlatın ve yeniden test edin.</span><span class="sxs-lookup"><span data-stu-id="6e4aa-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="6e4aa-105">Trafiği engelleyen Ağ Güvenlik Grupları (NSG) olup olmadığını belirlemek için VM'nizin ağ ayarlarını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="6e4aa-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="6e4aa-106">Ayrıca, Ağ [](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) İzleme aracını kullanarak trafiği engelleyen NSG'leri, trafiğinizi yeniden şirket içi yönlendirmeye ('Varsayılan Rota' 0.0.0.0/0) User-Defined Yönlendirmeleri'ne veya bir ağ cihazına yönlendirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6e4aa-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="6e4aa-107">Yukarıdaki adımları denemenin ardından sorun olmaya devam ediyorsanız, lütfen daha fazla tanı için posta göndermeye çalıştığınız VM adını ve TCP bağlantı noktasını girin.</span><span class="sxs-lookup"><span data-stu-id="6e4aa-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="6e4aa-108">**Önerilen Belgeler**</span><span class="sxs-lookup"><span data-stu-id="6e4aa-108">**Recommended Documents**</span></span>

[<span data-ttu-id="6e4aa-109">Bağlantı noktası 25 üzerinden giden e-posta göndermeye ilişkin sınırlamalar ve öneriler</span><span class="sxs-lookup"><span data-stu-id="6e4aa-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)