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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932463"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d3616-102">Kredi kartı numaraları ile DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="d3616-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d3616-103">**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor.</span><span class="sxs-lookup"><span data-stu-id="d3616-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d3616-104">Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır.</span><span class="sxs-lookup"><span data-stu-id="d3616-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d3616-105">Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.</span><span class="sxs-lookup"><span data-stu-id="d3616-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d3616-106">Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık.</span><span class="sxs-lookup"><span data-stu-id="d3616-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d3616-107">Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d3616-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d3616-108">Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.</span><span class="sxs-lookup"><span data-stu-id="d3616-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d3616-109">**Kredi kartı numaraları ile DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="d3616-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d3616-110">O365'te DLP duyarlı bilgi türü kullanırken **Kredi Kartı Numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="d3616-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d3616-111">Bu nedenle, içeriğinizin DLP ilkesini tetiklemek için gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="d3616-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d3616-112">Örneğin, %85 güven düzeyiyle yapılandırılan bir **Kredi Kartı politikası** için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="d3616-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d3616-113">**[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** Biçimlendirilebilir veya biçimlendirilmemiş (dddddddddddddddd) ve Luhn testini geçmek zorundadır 16 basamak.</span><span class="sxs-lookup"><span data-stu-id="d3616-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d3616-114">**[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa, MasterCard, Discover Card, JCB, American Express, hediye kartları ve yemek kartları dahil olmak üzere dünya çapındaki tüm büyük markaların kartlarını algılayan çok karmaşık ve sağlam desen.</span><span class="sxs-lookup"><span data-stu-id="d3616-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d3616-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Evet, Luhn çekleri.</span><span class="sxs-lookup"><span data-stu-id="d3616-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d3616-116">**[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:</span><span class="sxs-lookup"><span data-stu-id="d3616-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d3616-117">İşlev Func_credit_card desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="d3616-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d3616-118">Aşağıdakilerden biri doğrudur:</span><span class="sxs-lookup"><span data-stu-id="d3616-118">One of the following is true:</span></span>

  - <span data-ttu-id="d3616-119">Keyword_cc_verification'dan bir anahtar kelime bulunur.</span><span class="sxs-lookup"><span data-stu-id="d3616-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d3616-120">Keyword_cc_name'dan bir anahtar kelime bulundu</span><span class="sxs-lookup"><span data-stu-id="d3616-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d3616-121">İşlev Func_expiration_date doğru tarih biçiminde bir tarih bulur.</span><span class="sxs-lookup"><span data-stu-id="d3616-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d3616-122">Checksum geçer</span><span class="sxs-lookup"><span data-stu-id="d3616-122">The checksum passes</span></span>

    <span data-ttu-id="d3616-123">Örneğin, aşağıdaki örnek bir DLP Kredi Kartı Numarası Politikası için tetikler:</span><span class="sxs-lookup"><span data-stu-id="d3616-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d3616-124">Vize: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d3616-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d3616-125">Bitiş Tarihi: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d3616-125">Expires: 2/2009</span></span>

<span data-ttu-id="d3616-126">İçeriğiniz için kredi kartı **numarasının** algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri Kredi Kartı için ne arar#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d3616-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="d3616-127">Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d3616-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  