---
title: Genel geçiş performansı kılavuzu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932498"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="06d08-102">Genel geçiş performansı kılavuzu</span><span class="sxs-lookup"><span data-stu-id="06d08-102">General migration performance guidance</span></span>

<span data-ttu-id="06d08-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamaları çalıştırır. </span><span class="sxs-lookup"><span data-stu-id="06d08-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="06d08-104">Bunlar içerik geçişi, Veri Kaybı Önleme (DLP) ve yedekleme çözümlerini içerir.</span><span class="sxs-lookup"><span data-stu-id="06d08-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="06d08-105">Benzeri görünmemiş bu zamanlarda, uzaktan çalışma senaryolarında her zamankinden daha fazla hizmete bağımlı olan kullanıcılarınız için SharePoint Online ve OneDrive hizmetlerinin yüksek düzeyde kullanılabilir ve güvenilir olmaya devam etmesini sağlamaya yönelik bazı adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="06d08-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="06d08-106">Bu amacı desteklemek için hafta içi gündüz saatleri boyunca arka plan uygulamalarında (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma sınırları uyguladık.</span><span class="sxs-lookup"><span data-stu-id="06d08-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="06d08-107">Bu anlarda bu uygulamaların çok sınırlı işlem yapmasını beklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="06d08-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="06d08-108">Öte yandan, hizmet, bölgenin akşam ve hafta sonu saatleri boyunca arka plan uygulamalarından çok daha yüksek hacimde isteği işlemeye hazır olur.</span><span class="sxs-lookup"><span data-stu-id="06d08-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="06d08-109">**Geçiş performansı kılavuzu**</span><span class="sxs-lookup"><span data-stu-id="06d08-109">**Migration performance guidance**</span></span>

<span data-ttu-id="06d08-110">Ağ altyapısı, dosya boyutu, geçiş saati ve azaltma geçiş performansını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="06d08-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="06d08-111">Bunları anlamak, geçişinizi planlamanıza ve en üst düzeyde verimlilik elde etmenize yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="06d08-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="06d08-112">Genel geçiş performansı kılavuzu</span><span class="sxs-lookup"><span data-stu-id="06d08-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
