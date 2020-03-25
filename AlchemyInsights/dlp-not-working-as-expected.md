---
title: DLP beklendiği gibi çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932642"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e0444-102">DLP beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="e0444-102">DLP not working as expected</span></span>

<span data-ttu-id="e0444-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="e0444-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e0444-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="e0444-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e0444-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="e0444-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e0444-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="e0444-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e0444-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e0444-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e0444-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="e0444-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="e0444-109">**DLP'nin ayarlanması**</span><span class="sxs-lookup"><span data-stu-id="e0444-109">**Setting up DLP**</span></span>

<span data-ttu-id="e0444-110">Office 365'te **veri kaybının önlenmesi (DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="e0444-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e0444-111">Bu nedenle, **DLP ilkenizin** doğru şekilde ayarlandığınızdan ve verilerinizin **DLP ilkesinin** değerlendirilirken aradığı şeyi içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e0444-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e0444-112">DLP ilkeleri, kuruluşunuzdaki hassas bilgileri tanımlamanıza ve korumanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="e0444-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e0444-113">DLP ilkelerini kurmak için [buradaki](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="e0444-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e0444-114">**DLP ilkeleri ne leri arar**</span><span class="sxs-lookup"><span data-stu-id="e0444-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e0444-115">Office 365 Güvenlik ve Uyumluluk merkezinde **yerleşik hassas bilgi türlerini** kullanırken, DLP ilkeleri bu hassas türleri algılarken belirli desenleri ve öğeleri arar.</span><span class="sxs-lookup"><span data-stu-id="e0444-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e0444-116">**Yerleşik Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="e0444-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e0444-117">Yerleşik Hassas türleri ve Bir DLP ilkesinin Hassas türü algılarken ne aradığı hakkında bilgi için bkz: [Hassas bilgi türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)şey.</span><span class="sxs-lookup"><span data-stu-id="e0444-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e0444-118">**Özel Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="e0444-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e0444-119">Özel duyarlı bilgi türleri oluşturmaya çalışıyorsanız, özel duyarlı bir tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: [Özel duyarlı bilgi türü oluşturun.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="e0444-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e0444-120">**Bir DLP ilkesini test edin**</span><span class="sxs-lookup"><span data-stu-id="e0444-120">**Test a DLP policy**</span></span>

<span data-ttu-id="e0444-121">Verilerinizi yerleşik veya özel olarak duyarlı bilgi türüyle **sınamak** > için, Sınıflandırmalara**Duyarlı bilgi türleri**altında Test **türü** seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="e0444-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e0444-122">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="e0444-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e0444-123">**Raporlar**</span><span class="sxs-lookup"><span data-stu-id="e0444-123">**Reports**</span></span>
  
- <span data-ttu-id="e0444-124">[DLP Raporları](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) ile hassas veri öngörüleri alın.</span><span class="sxs-lookup"><span data-stu-id="e0444-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e0444-125">[Olay Raporu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)ile olayın belirli ayrıntılarını görün.</span><span class="sxs-lookup"><span data-stu-id="e0444-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
