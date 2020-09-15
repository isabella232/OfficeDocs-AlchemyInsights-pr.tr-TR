---
title: ABD banka hesap numarası için DLP kuralı çalışmıyor
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679316"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d0b32-102">ABD banka hesap numaralarıyla ilgili DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="d0b32-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="d0b32-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="d0b32-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d0b32-104">**ABD banka hesap numaralarıyla ilgili DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="d0b32-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="d0b32-105">O365 'de DLP duyarlı bir bilgi türü kullanırken, **ABD banka hesap numarası içeren bir ABD banka hesap numarası** içeren içerik Için çalışmayan **veri kaybı önleme (DLP)** sorunlarıyla karşılaşıyor musunuz?</span><span class="sxs-lookup"><span data-stu-id="d0b32-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d0b32-106">Bu durumda, içeriğinizin değerlendirilme sırasında hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="d0b32-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d0b32-107">Örneğin, %85 güvenilirlik düzeyiyle yapılandırılmış **US banka hesap numarası** ilkesinde, aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir:</span><span class="sxs-lookup"><span data-stu-id="d0b32-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d0b32-108">**[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 basamak</span><span class="sxs-lookup"><span data-stu-id="d0b32-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d0b32-109">**[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ardışık basamaklar.</span><span class="sxs-lookup"><span data-stu-id="d0b32-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d0b32-110">**[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, sağlama toplamı yok</span><span class="sxs-lookup"><span data-stu-id="d0b32-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d0b32-111">**[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %75.</span><span class="sxs-lookup"><span data-stu-id="d0b32-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d0b32-112">Normal ifade Regex_usa_bank_account_number desenle eşleşen içeriği bulur</span><span class="sxs-lookup"><span data-stu-id="d0b32-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d0b32-113">Keyword_usa_Bank_Account 'dan bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="d0b32-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d0b32-114">Örneğin, aşağıdaki örnek **ABD banka hesap numarası** ilkesini tetikleyecektir: hesap 78344011</span><span class="sxs-lookup"><span data-stu-id="d0b32-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d0b32-115">İçeriğiniz için bir **ABD banka hesap numarasının** gerekli olması gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne BAKıN: [ABD banka hesap numarası Için hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d0b32-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="d0b32-116">Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d0b32-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  