---
title: Takvim olayları eksik veya güncelleştiriliyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837587"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="4f8e1-102">Takvim Olayları eksik veya güncelleştiriliyor</span><span class="sxs-lookup"><span data-stu-id="4f8e1-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="4f8e1-103">Takvim öğeleri eksikse veya güncelleştirlenmiyorsa, Outlook'ta Takvim klasörü özelliklerinde öğe sayısına bakarak çalışmaya başlayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="4f8e1-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="4f8e1-104">Etkilenen kullanıcı Takvim klasörüne sağ **tıklayın** ve Özellikler'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="4f8e1-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="4f8e1-105">Eşitleme **sekmesini** seçin.</span><span class="sxs-lookup"><span data-stu-id="4f8e1-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="4f8e1-106">Sunucu klasörüyle Çevrimdışı Klasör arasında öğe sayısı aynıysa:</span><span class="sxs-lookup"><span data-stu-id="4f8e1-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="4f8e1-107">Takvim **klasörünü** vurgulayın.</span><span class="sxs-lookup"><span data-stu-id="4f8e1-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="4f8e1-108">Al Gönder  / **sekmesine gidin** ve Klasörü Güncelleştir'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="4f8e1-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="4f8e1-109">Takviminiz hala güncelleştiriliyorsa veya olaylar eksikse, Microsoft indirme merkezinden Outlook için Takvim [Denetleme Aracı'nı indirin.](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="4f8e1-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="4f8e1-110">Takvim klasöründe 5000'den fazla öğe olup olmadığını belirler çünkü bu durum takvim toplantıları gibi belirtilere veya toplantı hatalarına neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="4f8e1-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="4f8e1-111">Daha fazla bilgi için bkz. Önbelleğe alınmış modda [.ost](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)veya .pst dosyasında çok fazla öğe veya klasör olduğunda Outlook performans sorunları.</span><span class="sxs-lookup"><span data-stu-id="4f8e1-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>