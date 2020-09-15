---
title: SSN çalışmayan DLP kuralı
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679389"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="e6278-102">Sosyal güvenlik numaralarıyla ilgili DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="e6278-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="e6278-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="e6278-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e6278-104">**SSNs ile ilgili DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="e6278-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="e6278-105">Microsoft 365 'da hassas bir bilgi türü kullanırken bir **sosyal güvenlik numarası (SSK)** içeren içerik Için çalışmayan **veri kaybına KARŞı koruma (DLP** ) sorunlarıyla karşılaşmıyorsunuz mı?</span><span class="sxs-lookup"><span data-stu-id="e6278-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="e6278-106">Öyleyse, içeriğinizin, DLP ilkesinin hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e6278-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="e6278-107">Örneğin, %85 güvenirlik düzeyiyle yapılandırılmış bir SSN ilkesinde, aşağıdakiler değerlendirilir ve bu kural tetik için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="e6278-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e6278-108">**[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** biçimlendirilmiş veya biçimlendirilmemiş bir desende bulunan 9 basamak</span><span class="sxs-lookup"><span data-stu-id="e6278-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="e6278-109">**[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev, dört farklı görünümde SSNs arar:</span><span class="sxs-lookup"><span data-stu-id="e6278-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="e6278-110">Func_ssn, tire veya boşlukla biçimlendirilmiş, 2011 öncesi güçlü biçimlendirme ile SSNs bulur (ggg-gg-gggg veya ggg gg dddd)</span><span class="sxs-lookup"><span data-stu-id="e6278-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="e6278-111">2011 Func_unformatted_ssn, dokuz ardışık basamaklı (ggddddggg) biçimlendirilmemiş</span><span class="sxs-lookup"><span data-stu-id="e6278-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="e6278-112">Func_randomized_formatted_ssn, kısa çizgiler veya boşluklarla biçimlendirilmiş 2011 SSNs sonrası (ggg-gg-gggg veya ggg gg dddd) sözcüklerini bulur</span><span class="sxs-lookup"><span data-stu-id="e6278-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="e6278-113">Func_randomized_unformatted_ssn, dokuz ardışık rakamla biçimlendirilmemiş 2011 SSNs sonrası</span><span class="sxs-lookup"><span data-stu-id="e6278-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="e6278-114">**[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Hayır, sağlama toplamı yok</span><span class="sxs-lookup"><span data-stu-id="e6278-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="e6278-115">**[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %85.</span><span class="sxs-lookup"><span data-stu-id="e6278-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e6278-116">[İşlev Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="e6278-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e6278-117">[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) 'dan bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="e6278-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="e6278-118">Anahtar sözcük örnekleri:  *sosyal güvenlik, sosyal güvenlik #, SOC sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="e6278-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="e6278-119">Örneğin, aşağıdaki örnek DLP SSN ilkesi için tetikleyecektir: **SSK: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="e6278-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="e6278-120">İçeriğiniz için SSNs 'in algılanabilmesi gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="e6278-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="e6278-121">Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e6278-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  