---
title: İletilerin arşive otomatik olarak taşınmalarını durdurma
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527750"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="b81d3-102">İletilerin arşive otomatik olarak taşınmalarını durdurma</span><span class="sxs-lookup"><span data-stu-id="b81d3-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="b81d3-103">Bekletme ilkesi kullanıyorsanız, iletilerin otomatik olarak arşivlemesini durdurmak için bu ilkede bekletme yaşını değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b81d3-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="b81d3-104">Bunu şu şekilde yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b81d3-104">Here's how:</span></span>

1. <span data-ttu-id="b81d3-105">Exchange yönetim [merkezinde, uyumluluk](https://go.microsoft.com/fwlink/?linkid=2059104)yönetimi bekletme   >  **etiketlerini seçin.**</span><span class="sxs-lookup"><span data-stu-id="b81d3-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="b81d3-106">Arşive Taşı bekletme etiketinizi bulun.</span><span class="sxs-lookup"><span data-stu-id="b81d3-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="b81d3-107">Bekletme etiketinde, bekletme ilkesiyle öğelerin otomatik  olarak arşivlenmiş olmalarını durdurmak için bekletme dönemini (arşiv dönemi) Hiçbir zaman olarak değiştirme.</span><span class="sxs-lookup"><span data-stu-id="b81d3-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="b81d3-108">Bu, bu bekletme etiketinin uygulandığı tüm posta kutuları için arşiv ayarını değiştirir.</span><span class="sxs-lookup"><span data-stu-id="b81d3-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>