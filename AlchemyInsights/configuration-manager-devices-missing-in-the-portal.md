---
title: Portalda Yapılandırma Yöneticisi cihazları eksik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790237"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="da252-102">Portalda Yapılandırma Yöneticisi cihazları eksik</span><span class="sxs-lookup"><span data-stu-id="da252-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="da252-103">Cihaz eşitlemesinin gerçekleşmesi için, [gerekli Internet uç noktalarının](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) Hizmet Bağlantı Noktası rolüne sahip şirket içi sunucudan erişilebilir olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="da252-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="da252-104">Cihaz eşitlemesi sorunlarını gidermek için, lütfen hizmet bağlantı noktasında bulunan **CMGatewaySyncUploadWorker.log** dosyasını inceleyin.</span><span class="sxs-lookup"><span data-stu-id="da252-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="da252-105">[Microsoft Endpoint Manager’da Kiracı Ekleme](https://docs.microsoft.com/configmgr/tenant-attach/) hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="da252-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
