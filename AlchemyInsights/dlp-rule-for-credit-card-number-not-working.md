---
title: Kredi kartı numarası çalışmıyor DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389597"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="aa27f-102">Kredi kartı numaraları DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="aa27f-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="aa27f-103">**Veri kaybını önleme (DLP)** içinde O365 DLP hassas bilgi türünü kullanırken, bir **Kredi kartı numarası** içeren içerik için çalışmıyor sorun yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="aa27f-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="aa27f-104">Öyleyse, içeriğinizi tetiklemek için gerekli bilgileri içerdiğinden emin olun Bunu değerlendirildiğinde DLP ilkesi.</span><span class="sxs-lookup"><span data-stu-id="aa27f-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="aa27f-105">Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir **Kredi kartı İlkesi** , aşağıdaki değerlendirilir ve kural tetiklemek algılandı:</span><span class="sxs-lookup"><span data-stu-id="aa27f-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="aa27f-106">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** hangi biçimlendirilebilir 16 basamak veya biçimlendirilmemiş (dddddddddddddddd) ve Luhn sınamasından geçmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="aa27f-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="aa27f-107">**[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa, MasterCard, keşfedin kartı, JCB, American Express, hediye kartları ve diner kartları da dahil olmak üzere dünya çapında, tüm önemli markalar kartlardan algılar çok karmaşık ve güçlü deseni.</span><span class="sxs-lookup"><span data-stu-id="aa27f-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="aa27f-108">**[Sağlama toplamı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Evet, Luhn sağlama</span><span class="sxs-lookup"><span data-stu-id="aa27f-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="aa27f-109">**[Tanımı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Bu tür hassas bilgiler algıladı emin %85 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer:</span><span class="sxs-lookup"><span data-stu-id="aa27f-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="aa27f-110">Func_credit_card işlevi bir desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="aa27f-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="aa27f-111">Aşağıdakilerden biri doğrudur:</span><span class="sxs-lookup"><span data-stu-id="aa27f-111">One of the following is true:</span></span>

  - <span data-ttu-id="aa27f-112">Keyword_cc_verification herhangi bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="aa27f-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="aa27f-113">Keyword_cc_name herhangi bir anahtar sözcük bulunamadı</span><span class="sxs-lookup"><span data-stu-id="aa27f-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="aa27f-114">Func_expiration_date işlevi doğru tarih biçimindeki bir tarihi bulur.</span><span class="sxs-lookup"><span data-stu-id="aa27f-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="aa27f-115">Sağlama toplamı geçirir</span><span class="sxs-lookup"><span data-stu-id="aa27f-115">The checksum passes</span></span>

    <span data-ttu-id="aa27f-116">Örneğin, aşağıdaki örnek DLP kredi kartı numarası poliçesinin tetikler:</span><span class="sxs-lookup"><span data-stu-id="aa27f-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="aa27f-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="aa27f-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="aa27f-118">Son kullanma tarihi: 2/2009</span><span class="sxs-lookup"><span data-stu-id="aa27f-118">Expires: 2/2009</span></span>

<span data-ttu-id="aa27f-119">Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi bir **Kredi kartı numarası** için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgi aramak için kredi kartı # türleri](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="aa27f-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="aa27f-120">Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="aa27f-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  