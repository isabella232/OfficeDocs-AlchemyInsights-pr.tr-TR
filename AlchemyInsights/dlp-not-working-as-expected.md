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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707830"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="37240-102">DLP beklendiği gibi çalışmıyor</span><span class="sxs-lookup"><span data-stu-id="37240-102">DLP not working as expected</span></span>

<span data-ttu-id="37240-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="37240-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="37240-104">**DLP'i ayarlama**</span><span class="sxs-lookup"><span data-stu-id="37240-104">**Setting up DLP**</span></span>

<span data-ttu-id="37240-105">Office 365'te Veri **Kaybı Önleme (DLP)** ile ilgili sorunlar mı var?</span><span class="sxs-lookup"><span data-stu-id="37240-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="37240-106">Öyleyse, **DLP** ilkenizin doğru ayarlanmış olduğundan ve verilerinizin **DLP** ilkesi değerlendirilirken arayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="37240-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="37240-107">DLP ilkeleri, kuruluşta hassas bilgileri tanımlamanıza ve korumanıza olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="37240-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="37240-108">DLP ilkelerinin kurulumu için buradaki bilgileri [kullanın.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="37240-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="37240-109">**DLP ilkelerinin nasıl bir görünümde olduğu**</span><span class="sxs-lookup"><span data-stu-id="37240-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="37240-110">Güvenlik ve **Uyumluluk merkezlerinde yerleşik hassas** bilgi türleri kullanılırken, DLP ilkeleri bu hassas türleri algılarken belirli desenleri ve öğeleri aramalarına neden olur.</span><span class="sxs-lookup"><span data-stu-id="37240-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="37240-111">**Yerleşik Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="37240-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="37240-112">Yerleşik Hassas türler ve DLP ilkesi Hassas türünü algılarken nasıl arama yaptığını görmek için bkz. Hassas bilgi türleri [ne için arama yaptı.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="37240-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="37240-113">**Özel Hassas Bilgi Türleri**</span><span class="sxs-lookup"><span data-stu-id="37240-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="37240-114">Özel hassas bilgi türleri oluşturmaya çalışıyorsanız, özel hassas tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: Özel hassas [bilgi türü oluşturma.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="37240-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="37240-115">**DLP ilkesi test etmek**</span><span class="sxs-lookup"><span data-stu-id="37240-115">**Test a DLP policy**</span></span>

<span data-ttu-id="37240-116">Verilerinizi yerleşik veya özel bir hassas bilgi türüyle test etmek için Sınıflandırmalara Duyarlı bilgi türleri altındaki **Test** **türü**  >  **seçeneğini kullanın.**</span><span class="sxs-lookup"><span data-stu-id="37240-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="37240-117">Daha fazla bilgi için [bkz. Özel hassas bilgi türlerini test edin.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="37240-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="37240-118">**Raporlar**</span><span class="sxs-lookup"><span data-stu-id="37240-118">**Reports**</span></span>
  
- <span data-ttu-id="37240-119">DLP Raporları ile hassas [veri içgörüleri alın.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="37240-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="37240-120">Olay Raporu ile olayın belirli [ayrıntılarına bakın.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="37240-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
