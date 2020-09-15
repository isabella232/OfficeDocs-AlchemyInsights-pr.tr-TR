---
title: ABD/INGILTERE Passport numarası için DLP kuralı çalışmıyor
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679244"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c1365-102">DLP-US/INGILTERE Passport numaralarıyla ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="c1365-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c1365-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="c1365-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c1365-104">**ABD/INGILTERE Passport numaralarıyla DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="c1365-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c1365-105">O365 'de DLP duyarlı bir bilgi türü kullanırken, **ABD/İngiltere Passport numarası** içeren Içerik Için **veri kaybı önleme (DLP)** sorunlarıyla ilgili sorun mu yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="c1365-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c1365-106">Bu durumda, içeriğinizin değerlendirilme sırasında hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="c1365-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c1365-107">Örneğin, %75 güvenilirlik düzeyiyle yapılandırılmış **US/İngiltere Passport numarası** ilkesi için, aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir</span><span class="sxs-lookup"><span data-stu-id="c1365-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c1365-108">**[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dokuz basamak</span><span class="sxs-lookup"><span data-stu-id="c1365-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="c1365-109">**[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Art arda dokuz basamak</span><span class="sxs-lookup"><span data-stu-id="c1365-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c1365-110">**[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, sağlama toplamı yok</span><span class="sxs-lookup"><span data-stu-id="c1365-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c1365-111">**[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %75.</span><span class="sxs-lookup"><span data-stu-id="c1365-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c1365-112">İşlev Func_usa_uk_passport desenle eşleşen içeriği bulur.</span><span class="sxs-lookup"><span data-stu-id="c1365-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c1365-113">Keyword_passport 'dan bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="c1365-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c1365-114">Örneğin, aşağıdaki örnek **ABD/İngiltere Passport numarası** ilkesi için tetikleyecektir: ABD pasaport numarası 123456789</span><span class="sxs-lookup"><span data-stu-id="c1365-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c1365-115">İçeriğiniz için ABD/INGILTERE Passport numarasının gerekli olduğu hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [duyarlı bilgi türleri IÇIN ABD/Ingiltere Passport numarasını](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) görüntüleme</span><span class="sxs-lookup"><span data-stu-id="c1365-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c1365-116">Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c1365-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  