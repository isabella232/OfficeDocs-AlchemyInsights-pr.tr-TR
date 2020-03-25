---
title: Seçenekleri SharePoint Online'a geçirin
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932750"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="49e26-102">Seçenekleri SharePoint Online'a geçirin</span><span class="sxs-lookup"><span data-stu-id="49e26-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="49e26-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="49e26-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="49e26-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="49e26-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="49e26-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="49e26-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="49e26-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="49e26-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="49e26-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="49e26-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="49e26-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="49e26-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="49e26-109">**Geçiş seçenekleri**</span><span class="sxs-lookup"><span data-stu-id="49e26-109">**Migration options**</span></span>

<span data-ttu-id="49e26-110">İçeriği SharePoint Online'a geçirmek için farklı seçenekler vardır, taşımanız gereken dosyaların boyutuna ve miktarına bağlı olarak, lütfen [burada bulunan](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)seçeneklerin listesine bakın.</span><span class="sxs-lookup"><span data-stu-id="49e26-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="49e26-111">İçerik geçişi hakkında daha fazla bilgi için lütfen aşağıdaki bağlantıları ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="49e26-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="49e26-112">Sharepoint Geçiş Aracı</span><span class="sxs-lookup"><span data-stu-id="49e26-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="49e26-113">Geçiş Yöneticisi ile başlayın</span><span class="sxs-lookup"><span data-stu-id="49e26-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="49e26-114">Sharepoint Online ve ODB Geçiş Hızı</span><span class="sxs-lookup"><span data-stu-id="49e26-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="49e26-115">SharePoint Online'da daraltılmaktan veya engellenmesinden kaçının</span><span class="sxs-lookup"><span data-stu-id="49e26-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="49e26-116">SharePoint Geçiş Değerlendirme Aracı (SMAT)</span><span class="sxs-lookup"><span data-stu-id="49e26-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="49e26-117">**Not**: Şu anda SharePoint Geçiş aracı yalnızca SharePoint 2010 ve 2013'ten gelen geçişleri destekler.</span><span class="sxs-lookup"><span data-stu-id="49e26-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="49e26-118">Sürüm 2016 veya 2019 şu anda desteklenmez.</span><span class="sxs-lookup"><span data-stu-id="49e26-118">Version 2016 or 2019 are not supported at this time.</span></span>
