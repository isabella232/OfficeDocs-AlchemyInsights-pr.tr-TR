---
title: SSN için DLP kuralı çalışmıyor
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005002"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Sosyal Güvenlik Numaraları ile ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**SSN'lerle ilgili DLP sorunları**

SSN'de hassas bir bilgi türü kullanırken Veri Kaybı Önleme **(DLP) önleme (DLP)** içeren içerikte çalışmama sorunu mu Microsoft 365?  Varsa, içeriğinizin DLP ilkesine ilişkin gerekli bilgileri içerdiğindan emin olun. 
  
Örneğin, %85 güvenlik düzeyiyle yapılandırılmış bir SSN ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklesi için algılanır:
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** biçimlendirilmiş veya biçimlendirilmemiş bir desende 9 basamak

- **[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört farklı düzende SSN'ler için dört işlev bakın:

  - Func_ssn, tireler veya boşluklarla biçimlendirilmiş, 2011 öncesi güçlü biçimlendirmeye sahip SSN'leri (dd- dd- dddd VEYA daği biçimlendirilmiş) bulur

  - Func_unformatted_ssn sSN'leri 2011 öncesi, art arda dokuz basamaklı (ddddddddd) biçimlendirilmemiş, güçlü biçimlendirmeye sahip SSN'leri bulur

  - Func_randomized_formatted_ssn, tireler veya boşluklarla biçimlendirilmiş 2011 sonrası SSN'leri bulur (dd- dd- dddd VEYA daği biçimlendirilmiş SSN'ler)

  - Func_randomized_unformatted_ssn art arda dokuz basamaklı (dddddddd) olarak biçimlendirilmemiş 2011 sonrası SSN'leri bulur

- **[DenetimUmum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Hayır, Checksum yok

- **[Tanım:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP ilkesi, 300 karakter yakınlıkta olduğu durumda bu tür hassas bilgilerin algılandığından %85 emindir:

  - İşlev [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) desene eşleşen içeriği bulur.

  - Anahtar sözcük [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) bulunur. Anahtar sözcüklere örnek  *olarak: Sosyal Güvenlik, Sosyal Güvenlik#, Soc Sec ,SSN*  . Örneğin, aşağıdaki örnek DLP SSN İlkesini tetikler: **SSN: 489-36-8350**
  
İÇERIĞIniz için SSN'lerin algılandığında nelerin gerekli olduğu hakkında daha fazla bilgi için, bu makalenin şu bölümüne bakın: SSN'ler için Hassas Bilgi [Türleri'nin nasıl görünüyor?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Farklı bir yerleşik hassas bilgi türü kullanarak, diğer türlerde nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: Hassas Bilgi [Türleri'nin neleri araması](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  