---
title: SSN çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788722"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="02921-102">Sosyal Güvenlik Numaraları ile DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="02921-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="02921-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="02921-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="02921-104">**SSN'lerle DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="02921-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="02921-105">Microsoft 365'te hassas bir bilgi türünü kullanırken **Sosyal Güvenlik Numarası (SSN)** içeren içerik için çalışmayan Veri **KaybıÖnleme (DLP)** ile ilgili sorunlar yaşıyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="02921-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="02921-106">Bu nedenle, içeriğinizin DLP ilkesinin ne aradığına yönelik gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="02921-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="02921-107">Örneğin, %85 güven düzeyiyle yapılandırılan bir SSN ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="02921-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="02921-108">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** Biçimlendirilmiş veya biçimlendirilmemiş bir desende olabilecek 9 basamak</span><span class="sxs-lookup"><span data-stu-id="02921-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="02921-109">**[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev, SSN'leri dört farklı desende arar:</span><span class="sxs-lookup"><span data-stu-id="02921-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="02921-110">Func_ssn tire veya boşluk (ddd-dddd ddd dddd dddd) ile biçimlendirilmiş 2011 öncesi güçlü biçimlendirme ile SSN'ler bulur</span><span class="sxs-lookup"><span data-stu-id="02921-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="02921-111">Func_unformatted_ssn, art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 öncesi güçlü biçimlendirmeye sahip SSN'leri bulur</span><span class="sxs-lookup"><span data-stu-id="02921-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="02921-112">Func_randomized_formatted_ssn tire veya boşluk (ddd-dddd VEYA ddd dddd dddd) ile biçimlendirilmiş post-2011 SSNs bulur</span><span class="sxs-lookup"><span data-stu-id="02921-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="02921-113">Func_randomized_unformatted_ssn art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 sonrası SSN'leri bulur</span><span class="sxs-lookup"><span data-stu-id="02921-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="02921-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Hayır, Checksum diye bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="02921-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="02921-115">**[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:</span><span class="sxs-lookup"><span data-stu-id="02921-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="02921-116">İşlev [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="02921-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="02921-117">[Keyword_ssn'dan](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) bir anahtar kelime bulunur.</span><span class="sxs-lookup"><span data-stu-id="02921-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="02921-118">Anahtar kelimelere örnek olarak şunlar verilebilir: *Sosyal Güvenlik, Sosyal Güvenlik#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="02921-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="02921-119">Örneğin, Aşağıdaki örnek DLP SSN ilkesi için tetikler: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="02921-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="02921-120">İçeriğiniz için SSN'lerin algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri SSN'ler için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="02921-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="02921-121">Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="02921-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  