---
title: DLP beklendiği gibi çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679713"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="829ca-102">DLP beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="829ca-102">DLP not working as expected</span></span>

<span data-ttu-id="829ca-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="829ca-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="829ca-104">**DLP 'yi ayarlama**</span><span class="sxs-lookup"><span data-stu-id="829ca-104">**Setting up DLP**</span></span>

<span data-ttu-id="829ca-105">Office 365 'de **veri kaybı önleme (DLP)** ile ilgili sorun mu yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="829ca-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="829ca-106">Öyleyse, **DLP ilkenizin** doğru ayarlandığından ve verilerinizde **DLP ilkesinin** değerlendirilme sırasında hangi özelliklere sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="829ca-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="829ca-107">DLP ilkeleri kuruluşunuzdaki hassas bilgileri tanımlamanıza ve korumanızı sağlar.</span><span class="sxs-lookup"><span data-stu-id="829ca-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="829ca-108">DLP ilkelerini ayarlamak için [buradaki](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)bilgileri kullanın.</span><span class="sxs-lookup"><span data-stu-id="829ca-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="829ca-109">**Hangi DLP politikalarını arar**</span><span class="sxs-lookup"><span data-stu-id="829ca-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="829ca-110">Güvenlik ve uyumluluk merkezlerinde **yerleşik duyarlı bilgi türlerini** KULLANıRKEN, DLP ilkeleri bu hassas türleri algılayarak belirli desenleri ve öğeleri arar.</span><span class="sxs-lookup"><span data-stu-id="829ca-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="829ca-111">**Yerleşik duyarlı bilgi türleri**</span><span class="sxs-lookup"><span data-stu-id="829ca-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="829ca-112">Yerleşik duyarlı türler [ve duyarlı türü](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)algılayarak bir DLP İlkesi görünme hakkında bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="829ca-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="829ca-113">**Özel hassas bilgi türleri**</span><span class="sxs-lookup"><span data-stu-id="829ca-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="829ca-114">Özel hassas bilgi türleri oluşturmaya çalışıyorsanız, özel hassas bir tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: [özel hassas bilgi türü oluşturma](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="829ca-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="829ca-115">**DLP ilkesini sınama**</span><span class="sxs-lookup"><span data-stu-id="829ca-115">**Test a DLP policy**</span></span>

<span data-ttu-id="829ca-116">Verilerinizi yerleşik veya özel bir hassas bilgi türüyle sınamak için **Classifications**hassas bilgi türleri 'nin altındaki **test türü** seçeneğini kullanın  >  **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="829ca-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="829ca-117">Daha fazla bilgi [için bkz.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="829ca-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="829ca-118">**Raporlar**</span><span class="sxs-lookup"><span data-stu-id="829ca-118">**Reports**</span></span>
  
- <span data-ttu-id="829ca-119">[DLP raporlarıyla](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports) hassas veri öngörülerini edinin.</span><span class="sxs-lookup"><span data-stu-id="829ca-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="829ca-120">Olay [raporu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)ile olayın belirli ayrıntılarını görün.</span><span class="sxs-lookup"><span data-stu-id="829ca-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
