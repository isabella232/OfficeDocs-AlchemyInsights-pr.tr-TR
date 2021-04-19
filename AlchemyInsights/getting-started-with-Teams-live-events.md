---
title: Teams canlı etkinliklerini kullanmaya başlama
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811980"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="d13f8-102">Teams canlı etkinliklerini kullanmaya başlama</span><span class="sxs-lookup"><span data-stu-id="d13f8-102">Getting started with Teams live events</span></span>

<span data-ttu-id="d13f8-103">Microsoft Teams canlı etkinlikleri, kalabalık çevrimiçi kitlelere akış yapan etkinleri zamanlayıp oluşturmanızı sağlayan, Teams toplantılarının bir uzantısıdır.</span><span class="sxs-lookup"><span data-stu-id="d13f8-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="d13f8-104">Canlı etkinlik oluşturmak için şunlara ihtiyaç duyarsınız:</span><span class="sxs-lookup"><span data-stu-id="d13f8-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="d13f8-105">İlk olarak, Teams Canlı Etkinlikleri'nin Ülke [ve Bölgenize uygun olduğunu onaylayın](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Canlı Etkinlikler henüz bazı ülkelerde desteklenmiyor.</span><span class="sxs-lookup"><span data-stu-id="d13f8-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="d13f8-106">Lisans atadınız ve ilkeler ayardınız ancak yine de Teams Live Event oluşturamazsanız, büyük olasılıkla Canlı Etkinliklerin henüz kullanılabilir olmadığınız bir Ülke veya Bölgedesinizdir.</span><span class="sxs-lookup"><span data-stu-id="d13f8-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="d13f8-107">[Office 365 Kurumsal E1, E3 veya E5 lisansı ya da bir Office 365 A3 veya A5 lisansı](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="d13f8-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="d13f8-108">**Not**: Son zamanlarda Teams kullanımında görülen artış nedeniyle, bir kullanıcıya Teams lisansı atadığınızda kullanıcının çalışmaya tamamen hazır olması yaklaşık 24 saat sürebilir.</span><span class="sxs-lookup"><span data-stu-id="d13f8-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="d13f8-109">O zamana kadar bu kullanıcılara Teams ilkeleri atanamaz, kullanıcılar arama ve sesli konferans gibi bazı Teams özelliklerine erişemez.</span><span class="sxs-lookup"><span data-stu-id="d13f8-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="d13f8-110">[Microsoft Teams yönetim merkezinde canlı etkinlik oluşturma](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy) izni.</span><span class="sxs-lookup"><span data-stu-id="d13f8-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="d13f8-111">[Microsoft Stream’te canlı etkinlik oluşturma](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) izni (dış yayın uygulaması veya cihazı kullanılarak yapılan etkinlikler için).</span><span class="sxs-lookup"><span data-stu-id="d13f8-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="d13f8-112">Kuruluşta tam ekip üyeliği (misafir veya başka bir kuruluşun üyesi olamaz).</span><span class="sxs-lookup"><span data-stu-id="d13f8-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="d13f8-113">Özel toplantı zamanlama, ekran ve IP videosu paylaşma özelliklerinin Teams toplantı ilkesinde açık olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="d13f8-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="d13f8-114">Teams Canlı Etkinlikler için [en iyi uygulamalar](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42).</span><span class="sxs-lookup"><span data-stu-id="d13f8-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="d13f8-115">Daha fazla bilgi için bkz. [Microsoft Teams canlı etkinlikleri kullanmaya başlama](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="d13f8-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>