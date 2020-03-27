---
title: Geçiş Yöneticisi aracılığıyla SharePoint Online’a geçiş
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932376"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="fd292-102">Geçiş Yöneticisi aracılığıyla SharePoint Online’a geçiş</span><span class="sxs-lookup"><span data-stu-id="fd292-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="fd292-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamaları çalıştırır. </span><span class="sxs-lookup"><span data-stu-id="fd292-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="fd292-104">Bunlar içerik geçişi, Veri Kaybı Önleme (DLP) ve yedekleme çözümleridir.</span><span class="sxs-lookup"><span data-stu-id="fd292-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="fd292-105">Bu benzeri görünmemiş zamanlarda, uzaktan çalışma senaryolarında her zamankinden daha fazla hizmete bağımlı olan kullanıcılarınız için SharePoint Online ve OneDrive hizmetlerinin yüksek düzeyde kullanılabilir ve güvenilir olmaya devam etmesini sağlamaya yönelik bazı adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="fd292-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="fd292-106">Bu amacı desteklemek için, iş günlerinde gündüz saatleri boyunca arka plan uygulamalarında (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma sınırları uyguladık.</span><span class="sxs-lookup"><span data-stu-id="fd292-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="fd292-107">Bu zamanlarda bu uygulamaların çok sınırlı işlem yapmasını beklemelisiniz.</span><span class="sxs-lookup"><span data-stu-id="fd292-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="fd292-108">Öte yandan, bölge için akşam ve hafta sonu saatleri içinde hizmet, arka plan uygulamalarından çok daha yüksek hacimde isteği işlemeye hazır olur.</span><span class="sxs-lookup"><span data-stu-id="fd292-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="fd292-109">**Geçiş Yöneticisi**</span><span class="sxs-lookup"><span data-stu-id="fd292-109">**Migration Manager**</span></span>

<span data-ttu-id="fd292-110">Modern SharePoint Yönetim Merkezinde yer alan Geçiş Yöneticisi, istemcilerinizin kurulumunda ve görevlerinizin oluşturulması kapsamında size yol gösterir.</span><span class="sxs-lookup"><span data-stu-id="fd292-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="fd292-111">Küresel veya görev düzeyinde ayarları belirleyebilir, tüm görev ilerleme durumlarını görüntüleyebilir, toplu özet ve görev düzeyinde raporları indirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fd292-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="fd292-112">Geçiş Yöneticisiyle çalışmaya başlama</span><span class="sxs-lookup"><span data-stu-id="fd292-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="fd292-113">Geçiş Yöneticisi İstemcilerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="fd292-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="fd292-114">Geçiş Yöneticisi Ayarları</span><span class="sxs-lookup"><span data-stu-id="fd292-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
