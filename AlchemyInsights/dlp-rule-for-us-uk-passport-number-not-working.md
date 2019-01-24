---
title: DLP kuralı ABD / İngiltere Pasaport numarası çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494722"
---
<span data-ttu-id="a52af-p101">**Veri kaybını önleme (DLP)** içerik içeren için çalışmıyor ile sorunlarınız bir **ABD / İngiltere Pasaport numarası** içinde O365 DLP hassas bilgi türünü kullanırken? Öyleyse, emin olun, içeriğinizi onu değerlendirildiğinde DLP İlkesi aramak gerekli bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="a52af-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="a52af-104">Örneğin, bir **ABD / İngiltere Pasaport numarası** güvenirlik düzeyini % 75 ile yapılandırılan ilke, aşağıdaki değerlendirilir ve kural tetiklemek algılandı</span><span class="sxs-lookup"><span data-stu-id="a52af-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="a52af-105">**[Biçimi:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dokuz basamak</span><span class="sxs-lookup"><span data-stu-id="a52af-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="a52af-106">**[Desen:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Art arda dokuz basamak</span><span class="sxs-lookup"><span data-stu-id="a52af-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="a52af-107">**[Sağlama toplamı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, hiçbir sağlama yok</span><span class="sxs-lookup"><span data-stu-id="a52af-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="a52af-108">**[Tanımı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Bu tür hassas bilgiler algıladı emin % 75 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer:</span><span class="sxs-lookup"><span data-stu-id="a52af-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a52af-109">Func_usa_uk_passport işlevi bir desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="a52af-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="a52af-110">Keyword_passport herhangi bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="a52af-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="a52af-111">Örneğin, aşağıdaki örnek için tetikleyecektir **ABD / İngiltere Pasaport numarası** İlkesi: 123456789 ABD Pasaport numarası</span><span class="sxs-lookup"><span data-stu-id="a52af-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="a52af-112">Hakkında daha fazla bilgi için bir US gereklidir / İngiltere Pasaport numarası içeriğiniz için algılanabilmesi için bu makaledeki aşağıdaki bölümüne bakın: [ne hassas bilgi türlerini arayın, ABD / İngiltere Pasaport numarası](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a52af-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a52af-113">Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a52af-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

