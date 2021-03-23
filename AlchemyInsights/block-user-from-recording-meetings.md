---
title: Kullanıcının toplantıları kaydetmelerini engelleme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037065"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="0a7b1-102">Kullanıcının toplantıları kaydetmelerini engelleme</span><span class="sxs-lookup"><span data-stu-id="0a7b1-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="0a7b1-103">Belirli kullanıcıların Teams **Toplantıları kaydetmesini engellemeniz** veya engellemeniz gerekirse, bunu Teams Toplantı İlkesi ayarları aracılığıyla yapabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0a7b1-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="0a7b1-104">Microsoft Teams yönetim merkezinde, kullanıcıya atanan toplantı **ilkesinde** Bulut kaydına izin ver ayarını kapatın.</span><span class="sxs-lookup"><span data-stu-id="0a7b1-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="0a7b1-105">Daha fazla bilgi edinmek için [Teams'de toplantı ilkelerini yönetme'ye bakın.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="0a7b1-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="0a7b1-106">Belirli bir kullanıcının Teams Toplantıları kaydetmesine izin verili olup olmadığını doğrulamak için destek tanılamasını kullanın.</span><span class="sxs-lookup"><span data-stu-id="0a7b1-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="0a7b1-107">**Diag:** Toplantı Kaydı'nda yeni bir destek sorgusu çalıştırın ve bu sorguyu yazın; tanılama, belirtilen kullanıcının ilke ayarlarını kontrol edin ve ilke ayarlarını belirler.</span><span class="sxs-lookup"><span data-stu-id="0a7b1-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="0a7b1-108">Yeni ilke ayarlarının etkili bir şekilde yürürlüğe koyması birkaç saat sürebilir, dolayısıyla az önce bir değişiklik yaptıysanız, tanılamayı yeniden çalıştırmadan önce birkaç saat bekleyin.</span><span class="sxs-lookup"><span data-stu-id="0a7b1-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="0a7b1-109">Daha fazla bilgi için bulut [kaydını açma veya kapatmayı gözden geçirme.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="0a7b1-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
