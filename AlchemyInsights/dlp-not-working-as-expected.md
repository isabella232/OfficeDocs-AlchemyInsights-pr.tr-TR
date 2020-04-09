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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977458"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="cd6fa-102">DLP beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="cd6fa-102">DLP not working as expected</span></span>

<span data-ttu-id="cd6fa-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="cd6fa-104">**DLP'nin ayarlanması**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-104">**Setting up DLP**</span></span>

<span data-ttu-id="cd6fa-105">Office 365'te **veri kaybının önlenmesi (DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="cd6fa-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="cd6fa-106">Bu nedenle, **DLP ilkenizin** doğru şekilde ayarlandığınızdan ve verilerinizin **DLP ilkesinin** değerlendirilirken aradığı şeyi içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="cd6fa-107">DLP ilkeleri, kuruluşunuzdaki hassas bilgileri tanımlamanıza ve korumanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="cd6fa-108">DLP ilkelerini kurmak için [buradaki](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="cd6fa-109">**DLP ilkeleri ne leri arar**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="cd6fa-110">Office 365 Güvenlik ve Uyumluluk merkezinde **yerleşik hassas bilgi türlerini** kullanırken, DLP ilkeleri bu hassas türleri algılarken belirli desenleri ve öğeleri arar.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="cd6fa-111">**Yerleşik Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="cd6fa-112">Yerleşik Hassas türleri ve Bir DLP ilkesinin Hassas türü algılarken ne aradığı hakkında bilgi için bkz: [Hassas bilgi türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)şey.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="cd6fa-113">**Özel Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="cd6fa-114">Özel duyarlı bilgi türleri oluşturmaya çalışıyorsanız, özel duyarlı bir tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: [Özel duyarlı bilgi türü oluşturun.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="cd6fa-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="cd6fa-115">**Bir DLP ilkesini test edin**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-115">**Test a DLP policy**</span></span>

<span data-ttu-id="cd6fa-116">Verilerinizi yerleşik veya özel olarak duyarlı bilgi türüyle **sınamak** > için, Sınıflandırmalara**Duyarlı bilgi türleri**altında Test **türü** seçeneğini kullanın.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="cd6fa-117">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="cd6fa-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="cd6fa-118">**Raporlar**</span><span class="sxs-lookup"><span data-stu-id="cd6fa-118">**Reports**</span></span>
  
- <span data-ttu-id="cd6fa-119">[DLP Raporları](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) ile hassas veri öngörüleri alın.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="cd6fa-120">[Olay Raporu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)ile olayın belirli ayrıntılarını görün.</span><span class="sxs-lookup"><span data-stu-id="cd6fa-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
