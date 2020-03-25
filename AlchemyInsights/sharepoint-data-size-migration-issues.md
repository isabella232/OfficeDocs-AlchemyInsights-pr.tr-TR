---
title: Verileri SharePoint Online'a aktarırken sorunlar
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931714"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="28884-102">Verileri SharePoint Online'a aktarırken sorunlar</span><span class="sxs-lookup"><span data-stu-id="28884-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="28884-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="28884-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="28884-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="28884-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="28884-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="28884-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="28884-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="28884-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="28884-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="28884-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="28884-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="28884-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="28884-109">**100 TB'nin üzerinde veri geçirme**</span><span class="sxs-lookup"><span data-stu-id="28884-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="28884-110">SharePoint Online'a 100 TB'den fazla veri aktarıyor gibi görünüyorsunuz.</span><span class="sxs-lookup"><span data-stu-id="28884-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="28884-111">Lütfen aşağıdaki adımları uygulayın, böylece size en kısa sürede yardımcı olabiliriz.</span><span class="sxs-lookup"><span data-stu-id="28884-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="28884-112">**Yeni Hizmet İsteği'ni**ve ardından **Yeni Hizmet İsteği'ni**seçin.</span><span class="sxs-lookup"><span data-stu-id="28884-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="28884-113">**100 TB üzerinde SharePoint geçiş**olarak başlık ve açıklama bırakın.</span><span class="sxs-lookup"><span data-stu-id="28884-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="28884-114">Bilet gönderildikten sonra, lütfen aşağıdaki bilgilerle güncelleyin:</span><span class="sxs-lookup"><span data-stu-id="28884-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="28884-115">Geçişinizin tahmini boyutu.</span><span class="sxs-lookup"><span data-stu-id="28884-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="28884-116">Geçişinizi ne zaman başlatmak ve tamamlamak istediğinizin tahmini.</span><span class="sxs-lookup"><span data-stu-id="28884-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="28884-117">SharePoint Server, Box, GDrive, File shares, vb. gibi içeriğinizi nereden geçirdiğinizi açıklayın.</span><span class="sxs-lookup"><span data-stu-id="28884-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

