---
title: 503 hatayla sharePoint geçişi azaltma
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931678"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="5658f-102">503 hatayla sharePoint geçişi azaltma</span><span class="sxs-lookup"><span data-stu-id="5658f-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="5658f-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="5658f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5658f-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="5658f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5658f-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="5658f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5658f-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="5658f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5658f-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5658f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5658f-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="5658f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5658f-109">**SharePoint Online'a geçiş yaparken 503 hata**</span><span class="sxs-lookup"><span data-stu-id="5658f-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="5658f-110">SharePoint Online'a geçiş yapıyor ve 503 hata alıyor gibi görünüyor.</span><span class="sxs-lookup"><span data-stu-id="5658f-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="5658f-111">Lütfen aşağıdaki adımları uygulayın, böylece size en kısa sürede yardımcı olabiliriz.</span><span class="sxs-lookup"><span data-stu-id="5658f-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="5658f-112">**Destekle İlgili İletişim'i**ve ardından **Yeni Hizmet İsteği'ni**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="5658f-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="5658f-113">Başlık ve açıklama için **SharePoint Geçiş Azaltma yazısını 503 ile**.</span><span class="sxs-lookup"><span data-stu-id="5658f-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="5658f-114">Bilet gönderildikten sonra, lütfen aşağıdaki bilgilerle güncelleyin:</span><span class="sxs-lookup"><span data-stu-id="5658f-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="5658f-115">Geçişin ne kadarı kaldı (örneğin, kaç TB?).</span><span class="sxs-lookup"><span data-stu-id="5658f-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="5658f-116">Geçiş başlangıç ve bitiş tarihi.</span><span class="sxs-lookup"><span data-stu-id="5658f-116">Migration start and end date.</span></span>
    - <span data-ttu-id="5658f-117">SharePoint Server, Box, GDrive, File shares, vb. gibi içeriğinizi nereden geçirdiğinizi açıklayın.</span><span class="sxs-lookup"><span data-stu-id="5658f-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="5658f-118">Azaltma hatalarının sayısını (örneğin, saatte x azaltma?) ve azaltma ne zaman gerçekleştiğini tahmin edin.</span><span class="sxs-lookup"><span data-stu-id="5658f-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="5658f-119">Hangi geçiş aracını kullanıyorsunuz (örneğin, SPMT veya ShareGate).</span><span class="sxs-lookup"><span data-stu-id="5658f-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


