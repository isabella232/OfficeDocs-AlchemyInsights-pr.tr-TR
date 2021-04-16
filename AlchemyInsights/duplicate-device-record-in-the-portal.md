---
title: Portalda yinelenen cihaz kaydı
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
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814536"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="44e89-102">Portalda yinelenen cihaz kaydı</span><span class="sxs-lookup"><span data-stu-id="44e89-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="44e89-103">Bir cihaz, ortak yönetimi durumunu Configuration Manager sitesine doğru şekilde bildirmezse, portalda bir cihaza ait 2 kayıt görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="44e89-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="44e89-104">Cihazın ortak yönetim durumunu denetlemek için Configuration Manager konsolunda cihazın **Ortak yönetilen** sütununu gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="44e89-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="44e89-105">Sütun görünmüyorsa sütun başlıklarından herhangi birini sağ tıklayıp sütunu listeden seçerek ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="44e89-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="44e89-106">Ortak yönetilen değeri **Evet** olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="44e89-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="44e89-107">Değer **Hayır** ise istemci aygıtında Configuration Manager istemci uygulamasını açıp Genel sekmesindeki **Ortak yönetim** özelliğine bakın.</span><span class="sxs-lookup"><span data-stu-id="44e89-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="44e89-108">Değer **Etkin** ise bu, Yönetim Noktasıyla istemci iletişiminde sorun olduğunu gösterir.</span><span class="sxs-lookup"><span data-stu-id="44e89-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="44e89-109">Lütfen olası bağlantı sorunlarını araştırmak için cihazdaki **CcmMessaging.log** günlüğünü inceleyin.</span><span class="sxs-lookup"><span data-stu-id="44e89-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="44e89-110">Değer **Devre dışı** ise ve cihaz Intune’a kayıtlıysa, lütfen cihazdaki **CoManagementHandler.log** günlüğünü gözden geçirerek cihazın Ortak yönetim ilkesini aldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="44e89-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
