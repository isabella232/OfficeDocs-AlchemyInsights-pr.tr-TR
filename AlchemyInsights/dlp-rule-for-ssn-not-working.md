---
title: SSN çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932557"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="3b723-102">Sosyal Güvenlik Numaraları ile DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="3b723-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="3b723-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="3b723-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3b723-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="3b723-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3b723-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="3b723-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3b723-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="3b723-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3b723-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="3b723-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3b723-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="3b723-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3b723-109">**SSN'lerle DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="3b723-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="3b723-110">Office 365'te hassas bir bilgi türünü kullanırken **Sosyal Güvenlik Numarası (SSN)** içeren içerik için çalışmayan Veri **KaybıÖnleme (DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="3b723-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="3b723-111">Bu nedenle, içeriğinizin DLP ilkesinin ne aradığına yönelik gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="3b723-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="3b723-112">Örneğin, %85 güven düzeyiyle yapılandırılan bir SSN ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="3b723-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3b723-113">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** Biçimlendirilmiş veya biçimlendirilmemiş bir desende olabilecek 9 basamak</span><span class="sxs-lookup"><span data-stu-id="3b723-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="3b723-114">**[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev, SSN'leri dört farklı desende arar:</span><span class="sxs-lookup"><span data-stu-id="3b723-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="3b723-115">Func_ssn tire veya boşluk (ddd-dddd ddd dddd dddd) ile biçimlendirilmiş 2011 öncesi güçlü biçimlendirme ile SSN'ler bulur</span><span class="sxs-lookup"><span data-stu-id="3b723-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3b723-116">Func_unformatted_ssn, art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 öncesi güçlü biçimlendirmeye sahip SSN'leri bulur</span><span class="sxs-lookup"><span data-stu-id="3b723-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="3b723-117">Func_randomized_formatted_ssn tire veya boşluk (ddd-dddd VEYA ddd dddd dddd) ile biçimlendirilmiş post-2011 SSNs bulur</span><span class="sxs-lookup"><span data-stu-id="3b723-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3b723-118">Func_randomized_unformatted_ssn art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 sonrası SSN'leri bulur</span><span class="sxs-lookup"><span data-stu-id="3b723-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="3b723-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Hayır, Checksum diye bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="3b723-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="3b723-120">**[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:</span><span class="sxs-lookup"><span data-stu-id="3b723-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3b723-121">İşlev [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="3b723-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3b723-122">[Keyword_ssn'dan](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) bir anahtar kelime bulunur.</span><span class="sxs-lookup"><span data-stu-id="3b723-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="3b723-123">Anahtar kelimelere örnek olarak şunlar verilebilir: *Sosyal Güvenlik, Sosyal Güvenlik#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="3b723-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="3b723-124">Örneğin, Aşağıdaki örnek DLP SSN ilkesi için tetikler: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="3b723-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="3b723-125">İçeriğiniz için SSN'lerin algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri SSN'ler için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="3b723-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="3b723-126">Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3b723-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  