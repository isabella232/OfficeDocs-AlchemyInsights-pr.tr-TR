---
title: SSN çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788722"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Sosyal Güvenlik Numaraları ile DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**SSN'lerle DLP sorunları**

Microsoft 365'te hassas bir bilgi türünü kullanırken **Sosyal Güvenlik Numarası (SSN)** içeren içerik için çalışmayan Veri **KaybıÖnleme (DLP)** ile ilgili sorunlar yaşıyor musunuz? Bu nedenle, içeriğinizin DLP ilkesinin ne aradığına yönelik gerekli bilgileri içerdiğinden emin olun. 
  
Örneğin, %85 güven düzeyiyle yapılandırılan bir SSN ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:
  
- **[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** Biçimlendirilmiş veya biçimlendirilmemiş bir desende olabilecek 9 basamak

- **[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev, SSN'leri dört farklı desende arar:

  - Func_ssn tire veya boşluk (ddd-dddd ddd dddd dddd) ile biçimlendirilmiş 2011 öncesi güçlü biçimlendirme ile SSN'ler bulur

  - Func_unformatted_ssn, art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 öncesi güçlü biçimlendirmeye sahip SSN'leri bulur

  - Func_randomized_formatted_ssn tire veya boşluk (ddd-dddd VEYA ddd dddd dddd) ile biçimlendirilmiş post-2011 SSNs bulur

  - Func_randomized_unformatted_ssn art arda dokuz basamak (ddddddddd) olarak biçimlendirilmemiş 2011 sonrası SSN'leri bulur

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Hayır, Checksum diye bir şey yok.

- **[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:

  - İşlev [Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) desenle eşleşen içeriği bulur.

  - [Keyword_ssn'dan](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) bir anahtar kelime bulunur. Anahtar kelimelere örnek olarak şunlar verilebilir: *Sosyal Güvenlik, Sosyal Güvenlik#, Soc Sec ,SSN* . Örneğin, Aşağıdaki örnek DLP SSN ilkesi için tetikler: **SSN: 489-36-8350**
  
İçeriğiniz için SSN'lerin algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri SSN'ler için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  