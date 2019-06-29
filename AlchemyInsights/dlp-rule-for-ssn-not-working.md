---
title: DLP kuralı SSN çalışmıyor
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389453"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="5e2dd-102">Sosyal Güvenlik numaraları DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="5e2dd-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="5e2dd-103">Office 365'de hassas bilgi türünü kullanırken, bir **Sosyal güvenlik numarası (SSK)** içeren içerik için çalışmıyor **Veri kaybını önleme (DLP)** ile ilgili sorunlar yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="5e2dd-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="5e2dd-104">Öyleyse, içeriğinizi DLP İlkesi ne arıyor için gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="5e2dd-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="5e2dd-105">Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir SSN ilke için aşağıdaki değerlendirilir ve kural tetiklemek algılandı:</span><span class="sxs-lookup"><span data-stu-id="5e2dd-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="5e2dd-106">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** biçimlendirilmiş veya biçimlendirilmemiş bir desende olabilen 9 basamak</span><span class="sxs-lookup"><span data-stu-id="5e2dd-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="5e2dd-107">**[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev dört farklı desenler SSNs için arayın:</span><span class="sxs-lookup"><span data-stu-id="5e2dd-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="5e2dd-108">Func_ssn öncesi 2011 güçlü tire veya boşluk (ggg gg gggg OR ggg gg dddd) ile biçimlendirilmiş biçimlendirme ile SSNs bulur.</span><span class="sxs-lookup"><span data-stu-id="5e2dd-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="5e2dd-109">Func_unformatted_ssn öncesi 2011 güçlü dokuz ardışık rakamlar (ddddddddd) biçimlendirilmemiş olan biçimlendirme ile SSNs bulur.</span><span class="sxs-lookup"><span data-stu-id="5e2dd-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="5e2dd-110">Tire veya boşluk (ggg gg gggg OR ggg gg dddd) ile biçimlendirilmiş bir post-2011 SSNs Func_randomized_formatted_ssn bulur</span><span class="sxs-lookup"><span data-stu-id="5e2dd-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="5e2dd-111">Dokuz ardışık rakamlar (ddddddddd) biçimlendirilmemiş post-2011 SSNs Func_randomized_unformatted_ssn bulur</span><span class="sxs-lookup"><span data-stu-id="5e2dd-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="5e2dd-112">**[Sağlama toplamı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Hayır, hiçbir sağlama yok</span><span class="sxs-lookup"><span data-stu-id="5e2dd-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="5e2dd-113">**[Tanımı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Bu tür hassas bilgiler algıladı emin %85 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer:</span><span class="sxs-lookup"><span data-stu-id="5e2dd-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5e2dd-114">[Func_ssn işlevi](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) bir desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="5e2dd-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5e2dd-115">[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) herhangi bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="5e2dd-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="5e2dd-116">Anahtar sözcük örnekleri içerir: *sosyal güvenlik, sosyal güvenlik #, Soc sn, SSN* .</span><span class="sxs-lookup"><span data-stu-id="5e2dd-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="5e2dd-117">Örneğin, aşağıdaki örnek DLP SSN poliçesinin tetikleyecektir: **SSK: 489 36 8350**</span><span class="sxs-lookup"><span data-stu-id="5e2dd-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="5e2dd-118">Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi SSNs için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgi aramak için SSNs türleri](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="5e2dd-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="5e2dd-119">Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5e2dd-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  