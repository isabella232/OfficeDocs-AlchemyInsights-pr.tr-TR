---
title: Kredi kartı numarası için DLP kuralı çalışmıyor
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679461"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d20b2-102">Kredi kartı numaralarıyla ilgili DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="d20b2-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d20b2-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="d20b2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d20b2-104">**Kredi kartı numaralarıyla ilgili DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="d20b2-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d20b2-105">O365 'de DLP duyarlı bir bilgi türü kullanırken, **kredi kartı numarası** içeren Içerik Için **veri kaybı önleme (DLP)** sorunlarıyla karşılaşmıyorsunuz mı?</span><span class="sxs-lookup"><span data-stu-id="d20b2-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d20b2-106">Bu durumda, içeriğinizin değerlendirilme sırasında DLP ilkesini tetiklemek için gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="d20b2-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d20b2-107">Örneğin, %85 güvenilirlik düzeyiyle yapılandırılmış bir **kredi kartı ilkesinde** , aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="d20b2-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d20b2-108">**[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** biçimlendirilebilen veya biçimlendirilmemiş (dddddddddddddddd) 16 basamak.</span><span class="sxs-lookup"><span data-stu-id="d20b2-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d20b2-109">**[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Visa, MasterCard, keşif kartı, JCB, Amerikan Express, hediye kartları ve Diner kartları dahil tüm dünya genelindeki tüm önemli markalardan kartlar algılayan çok karmaşık ve güçlü bir düzen.</span><span class="sxs-lookup"><span data-stu-id="d20b2-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d20b2-110">**[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Evet, Luhn sağlaması</span><span class="sxs-lookup"><span data-stu-id="d20b2-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d20b2-111">**[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %85.</span><span class="sxs-lookup"><span data-stu-id="d20b2-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d20b2-112">İşlev Func_credit_card desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="d20b2-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d20b2-113">Aşağıdakilerden biri doğrudur:</span><span class="sxs-lookup"><span data-stu-id="d20b2-113">One of the following is true:</span></span>

  - <span data-ttu-id="d20b2-114">Keyword_cc_verification 'dan bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="d20b2-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d20b2-115">Keyword_cc_name 'dan bir anahtar sözcük bulundu</span><span class="sxs-lookup"><span data-stu-id="d20b2-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d20b2-116">İşlev Func_expiration_date, sağ tarih biçiminde bir tarih bulur.</span><span class="sxs-lookup"><span data-stu-id="d20b2-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d20b2-117">Sağlama toplamı geçişlerinde</span><span class="sxs-lookup"><span data-stu-id="d20b2-117">The checksum passes</span></span>

    <span data-ttu-id="d20b2-118">Örneğin, aşağıdaki örnek bir DLP kredi kartı numarası Ilkesi için tetikleyecektir:</span><span class="sxs-lookup"><span data-stu-id="d20b2-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d20b2-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d20b2-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d20b2-120">Süre sonu: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d20b2-120">Expires: 2/2009</span></span>

<span data-ttu-id="d20b2-121">İçeriğiniz için bir **kredi kartı numarasının** gerekli olması gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [kredi kartı # Için hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d20b2-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="d20b2-122">Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d20b2-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  