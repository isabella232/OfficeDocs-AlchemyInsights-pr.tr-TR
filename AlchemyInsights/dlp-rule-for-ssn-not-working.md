---
title: SSN çalışmayan DLP kuralı
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679389"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Sosyal güvenlik numaralarıyla ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**SSNs ile ilgili DLP sorunları**

Microsoft 365 'da hassas bir bilgi türü kullanırken bir **sosyal güvenlik numarası (SSK)** içeren içerik Için çalışmayan **veri kaybına KARŞı koruma (DLP** ) sorunlarıyla karşılaşmıyorsunuz mı? Öyleyse, içeriğinizin, DLP ilkesinin hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun. 
  
Örneğin, %85 güvenirlik düzeyiyle yapılandırılmış bir SSN ilkesinde, aşağıdakiler değerlendirilir ve bu kural tetik için algılanmalıdır:
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** biçimlendirilmiş veya biçimlendirilmemiş bir desende bulunan 9 basamak

- **[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev, dört farklı görünümde SSNs arar:

  - Func_ssn, tire veya boşlukla biçimlendirilmiş, 2011 öncesi güçlü biçimlendirme ile SSNs bulur (ggg-gg-gggg veya ggg gg dddd)

  - 2011 Func_unformatted_ssn, dokuz ardışık basamaklı (ggddddggg) biçimlendirilmemiş

  - Func_randomized_formatted_ssn, kısa çizgiler veya boşluklarla biçimlendirilmiş 2011 SSNs sonrası (ggg-gg-gggg veya ggg gg dddd) sözcüklerini bulur

  - Func_randomized_unformatted_ssn, dokuz ardışık rakamla biçimlendirilmemiş 2011 SSNs sonrası

- **[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Hayır, sağlama toplamı yok

- **[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %85.

  - [İşlev Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) desenle eşleşen içeriği bulur.

  - [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) 'dan bir anahtar sözcük bulundu. Anahtar sözcük örnekleri:  *sosyal güvenlik, sosyal güvenlik #, SOC sec, SSN*  . Örneğin, aşağıdaki örnek DLP SSN ilkesi için tetikleyecektir: **SSK: 489-36-8350**
  
İçeriğiniz için SSNs 'in algılanabilmesi gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  