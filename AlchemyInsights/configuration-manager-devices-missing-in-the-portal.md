---
title: Portalda Yapılandırma Yöneticisi cihazları eksik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817264"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="51a13-102">Portalda Yapılandırma Yöneticisi cihazları eksik</span><span class="sxs-lookup"><span data-stu-id="51a13-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="51a13-103">Cihaz eşitlemesinin gerçekleşmesi için, [gerekli Internet uç noktalarının](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) Hizmet Bağlantı Noktası rolüne sahip şirket içi sunucudan erişilebilir olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="51a13-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="51a13-104">Cihaz eşitlemesi sorunlarını gidermek için, lütfen hizmet bağlantı noktasında bulunan **CMGatewaySyncUploadWorker.log** dosyasını inceleyin.</span><span class="sxs-lookup"><span data-stu-id="51a13-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="51a13-105">[Microsoft Endpoint Manager’da Kiracı Ekleme](https://docs.microsoft.com/configmgr/tenant-attach/) hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="51a13-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
