---
title: Yammer’da canlı etkinlik oluşturma hataları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948022"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="fc2f3-102">Yammer’da canlı etkinlik oluşturma hataları</span><span class="sxs-lookup"><span data-stu-id="fc2f3-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="fc2f3-103">**Yammer Canlı Etkinlik oluşturma**</span><span class="sxs-lookup"><span data-stu-id="fc2f3-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="fc2f3-104">Yammer canlı etkinlik oluşturma seçeneğini sürekli gösterir.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="fc2f3-105">Bazı durumlarda bir kullanıcı canlı etkinlik oluşturmanın önkoşullarını karşılamayabilir ve oluşturmayı denediğinde hata alabilir.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="fc2f3-106">Aşağıdaki öğeler bu sorunun yaygın nedenlerini kapsar ve son kullanıcılar için bunlar çözmenin yollarını sağlar.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="fc2f3-107">**Kimler canlı etkinlik oluşturabilir?**</span><span class="sxs-lookup"><span data-stu-id="fc2f3-107">**Who can create live events**</span></span>
- <span data-ttu-id="fc2f3-108">Office 365 Kurumsal E1, E3 veya E5 lisansı ya da bir Office 365 A3 veya A5 lisansı.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="fc2f3-109">Microsoft Teams yönetim merkezinde canlı etkinlik oluşturma izni.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="fc2f3-110">Microsoft Stream’te canlı etkinlik oluşturma izni (dış yayın uygulaması veya cihazı kullanılarak yapılan etkinlikler için).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="fc2f3-111">Kuruluşta tam ekip üyeliği (misafir veya başka bir kuruluşun üyesi olamaz).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="fc2f3-112">Özel toplantı zamanlama, ekran ve IP videosu paylaşma özelliklerinin Teams toplantı ilkesinde açık olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="fc2f3-113">**Canlı etkinlik oluşturma ilkeleri**</span><span class="sxs-lookup"><span data-stu-id="fc2f3-113">**Live event creation policies**</span></span>

<span data-ttu-id="fc2f3-114">Yammer, Office 365 kiracınızda Stream için ayarlanan Canlık Etkinlik ilkelerine uyar.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="fc2f3-115">Varsayılan olarak kuruluşunuzdaki herkes canlı etkinlik oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="fc2f3-116">Yöneticiler [bu ayarda kullanıcıların canlı etkinlik oluşturmasını engelleyebilecek değişiklikler yapabilir](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="fc2f3-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="fc2f3-117">İlke hatası alan kullanıcıların canlı etkinlik oluşturma izinleri olup olmadığını denetlemek önemlidir.</span><span class="sxs-lookup"><span data-stu-id="fc2f3-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
