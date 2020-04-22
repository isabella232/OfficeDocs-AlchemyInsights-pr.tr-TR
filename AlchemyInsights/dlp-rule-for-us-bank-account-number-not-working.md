---
title: ABD Banka Hesap Numarası çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704059"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a5d50-102">ABD banka hesap numaraları ile DLP sorunları</span><span class="sxs-lookup"><span data-stu-id="a5d50-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a5d50-103">**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="a5d50-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a5d50-104">**ABD banka hesap numaraları ile DLP sorunları**</span><span class="sxs-lookup"><span data-stu-id="a5d50-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a5d50-105">O365'te DLP'ye duyarlı bilgi türünü kullanırken **ABD Banka Hesap Numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="a5d50-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a5d50-106">Bu nedenle, içeriğinizin DLP ilkesinin değerlendirildiğinde aradığı bilgiler için gerekli bilgileri içerdiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="a5d50-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a5d50-107">Örneğin, %85 güven düzeyiyle yapılandırılan bir **ABD Banka Hesap Numarası** ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:</span><span class="sxs-lookup"><span data-stu-id="a5d50-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a5d50-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 basamak</span><span class="sxs-lookup"><span data-stu-id="a5d50-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a5d50-109">**[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ardışık basamak.</span><span class="sxs-lookup"><span data-stu-id="a5d50-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a5d50-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, Checksum diye bir şey yok.</span><span class="sxs-lookup"><span data-stu-id="a5d50-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a5d50-111">**[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %75 emindir:</span><span class="sxs-lookup"><span data-stu-id="a5d50-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a5d50-112">Normal ifade Regex_usa_bank_account_number desenle eşleşen içeriği bulur</span><span class="sxs-lookup"><span data-stu-id="a5d50-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a5d50-113">Keyword_usa_Bank_Account'dan bir anahtar kelime bulunur.</span><span class="sxs-lookup"><span data-stu-id="a5d50-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a5d50-114">Örneğin, AŞAĞıDAKI örnek **ABD Banka Hesap Numarası** politikası için tetikleyeceği gibi: Çek Hesabı 78344011</span><span class="sxs-lookup"><span data-stu-id="a5d50-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a5d50-115">İçeriğiniz için bir ABD **Banka Hesap Numarasının** algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri ABD Banka Hesap Numarası için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="a5d50-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="a5d50-116">Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a5d50-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  