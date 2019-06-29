---
title: DLP kural numaralı BİZE banka hesabı çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389489"
---
<span data-ttu-id="14974-102">**Veri kaybını önleme (DLP)** içinde O365 DLP hassas bilgi türünü kullanırken, bir **ABD banka hesap numarasını** içeren içerik için çalışmıyor sorun yaşıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="14974-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="14974-103">Öyleyse, emin olun, içeriğinizi onu değerlendirildiğinde DLP İlkesi aramak gerekli bilgileri içerir.</span><span class="sxs-lookup"><span data-stu-id="14974-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="14974-104">Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir **ABD banka hesap numarası** ilke için aşağıdaki değerlendirilir ve kural tetiklemek algılandı:</span><span class="sxs-lookup"><span data-stu-id="14974-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="14974-105">**[Biçimi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 basamak</span><span class="sxs-lookup"><span data-stu-id="14974-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="14974-106">**[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ardışık rakamlar.</span><span class="sxs-lookup"><span data-stu-id="14974-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="14974-107">**[Sağlama toplamı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, hiçbir sağlama yok</span><span class="sxs-lookup"><span data-stu-id="14974-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="14974-108">**[Tanımı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Bu tür hassas bilgiler algıladı emin % 75 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer:</span><span class="sxs-lookup"><span data-stu-id="14974-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="14974-109">Desenle eşleşen içerik Regex_usa_bank_account_number normal ifade bulur</span><span class="sxs-lookup"><span data-stu-id="14974-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="14974-110">Keyword_usa_Bank_Account herhangi bir anahtar sözcük bulundu.</span><span class="sxs-lookup"><span data-stu-id="14974-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="14974-111">Örneğin, aşağıdaki örnek **ABD banka hesap numarası** poliçesinin tetikleyecektir: Çek Hesabı 78344011</span><span class="sxs-lookup"><span data-stu-id="14974-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="14974-112">Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi **ABD banka hesap numarası** için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgileri ABD banka hesap numarası için arama türleri](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="14974-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="14974-113">Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="14974-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  