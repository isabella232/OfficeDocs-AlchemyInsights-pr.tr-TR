---
title: DLP sorunları hakkında daha fazla bilgi
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932714"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="ebfc7-102">DLP sorunları hakkında bilgi</span><span class="sxs-lookup"><span data-stu-id="ebfc7-102">Information about DLP issues</span></span>

<span data-ttu-id="ebfc7-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ebfc7-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ebfc7-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ebfc7-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ebfc7-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ebfc7-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ebfc7-109">**DLP ilkesi hakkında bilgi**</span><span class="sxs-lookup"><span data-stu-id="ebfc7-109">**Information on DLP policy**</span></span>

<span data-ttu-id="ebfc7-110">Bir DLP ilkesiyle, Office 365 genelinde hassas bilgileri tanımlayabilir, izleyebilir ve otomatik olarak koruyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="ebfc7-111">Daha fazla bilgi için lütfen bu bağlantıları ziyaret edin:</span><span class="sxs-lookup"><span data-stu-id="ebfc7-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="ebfc7-112">Veri kaybı önlemeye genel bakış</span><span class="sxs-lookup"><span data-stu-id="ebfc7-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="ebfc7-113">Hassas bilgi türlerinin aradığı</span><span class="sxs-lookup"><span data-stu-id="ebfc7-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="ebfc7-114">Özel duyarlı bilgi türü oluşturma</span><span class="sxs-lookup"><span data-stu-id="ebfc7-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="ebfc7-115">E-posta bildirimleri gönderme ve ilke ipuçlarını gösterme</span><span class="sxs-lookup"><span data-stu-id="ebfc7-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="ebfc7-116">SharePoint Online dosyalarını bekletme etiketleri ve DLP ile koruma</span><span class="sxs-lookup"><span data-stu-id="ebfc7-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="ebfc7-117">DLP ve Microsoft Ekipleri</span><span class="sxs-lookup"><span data-stu-id="ebfc7-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="ebfc7-118">Verilerinizi yerleşik veya özel olarak duyarlı bilgi türüyle **sınamak** > için, Sınıflandırmalara**Duyarlı bilgi türleri**altında Test **türü** seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="ebfc7-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ebfc7-119">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="ebfc7-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>