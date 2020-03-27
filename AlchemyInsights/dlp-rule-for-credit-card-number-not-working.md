---
title: Kredi Kartı Numarası çalışmıyor için DLP Kuralı
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977218"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="e9766-102">Kredi kartı numaraları ile DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="e9766-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="e9766-103">**Önemli**: Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin yüksek oranda kullanılabilir kalmasını sağlamak için adımlar atıyoruz – Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Ayarlamaları'nı](https://aka.ms/ODSPAdjustments) ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="e9766-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e9766-104">**Kredi kartı numaraları ile DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="e9766-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="e9766-105">O365'te DLP duyarlı bilgi türü kullanırken **Kredi Kartı Numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="e9766-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e9766-106">Bu nedenle, içeriğinizin DLP ilkesini tetiklemek için gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e9766-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="e9766-107">Örneğin, %85 güven düzeyiyle yapılandırılan bir **Kredi Kartı politikası** için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="e9766-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e9766-108">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** Biçimlendirilebilir veya biçimlendirilmemiş (dddddddddddddddd) ve Luhn testini geçmek zorundadır 16 basamak.</span><span class="sxs-lookup"><span data-stu-id="e9766-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="e9766-109">**[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa, MasterCard, Discover Card, JCB, American Express, hediye kartları ve yemek kartları dahil olmak üzere dünya çapındaki tüm büyük markaların kartlarını algılayan çok karmaşık ve sağlam desen.</span><span class="sxs-lookup"><span data-stu-id="e9766-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="e9766-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Evet, Luhn çekleri.</span><span class="sxs-lookup"><span data-stu-id="e9766-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="e9766-111">**[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:</span><span class="sxs-lookup"><span data-stu-id="e9766-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e9766-112">İşlev Func_credit_card desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="e9766-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e9766-113">Aşağıdakilerden biri doğrudur:</span><span class="sxs-lookup"><span data-stu-id="e9766-113">One of the following is true:</span></span>

  - <span data-ttu-id="e9766-114">Keyword_cc_verification'dan bir anahtar kelime bulunur.</span><span class="sxs-lookup"><span data-stu-id="e9766-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="e9766-115">Keyword_cc_name'dan bir anahtar kelime bulundu</span><span class="sxs-lookup"><span data-stu-id="e9766-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="e9766-116">İşlev Func_expiration_date doğru tarih biçiminde bir tarih bulur.</span><span class="sxs-lookup"><span data-stu-id="e9766-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="e9766-117">Checksum geçer</span><span class="sxs-lookup"><span data-stu-id="e9766-117">The checksum passes</span></span>

    <span data-ttu-id="e9766-118">Örneğin, aşağıdaki örnek bir DLP Kredi Kartı Numarası Politikası için tetikler:</span><span class="sxs-lookup"><span data-stu-id="e9766-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="e9766-119">Vize: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e9766-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="e9766-120">Bitiş Tarihi: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e9766-120">Expires: 2/2009</span></span>

<span data-ttu-id="e9766-121">İçeriğiniz için kredi kartı **numarasının** algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri Kredi Kartı için ne arar#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e9766-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="e9766-122">Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e9766-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  