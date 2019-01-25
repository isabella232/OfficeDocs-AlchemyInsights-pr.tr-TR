---
title: DLP kuralı SSN çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495192"
---
Office 365'de hassas bilgi türünü kullanırken, bir **Sosyal güvenlik numarası (SSK)** içeren içerik için çalışmıyor **Veri kaybını önleme (DLP)** ile ilgili sorunlar yaşıyorsunuz? Öyleyse, içeriğinizi DLP İlkesi ne arıyor için gerekli bilgileri içerdiğinden emin olun. 
  
Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir SSN ilke için aşağıdaki değerlendirilir ve kural tetiklemek algılandı:
  
- **[Biçim:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** biçimlendirilmiş veya biçimlendirilmemiş bir desende olabilen 9 basamak 
    
- **[Desen:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Dört işlev dört farklı desenler SSNs için arayın: 
    
  - Func_ssn öncesi 2011 güçlü tire veya boşluk (ggg gg gggg OR ggg gg dddd) ile biçimlendirilmiş biçimlendirme ile SSNs bulur.
    
  - Func_unformatted_ssn öncesi 2011 güçlü dokuz ardışık rakamlar (ddddddddd) biçimlendirilmemiş olan biçimlendirme ile SSNs bulur.
    
  - Tire veya boşluk (ggg gg gggg OR ggg gg dddd) ile biçimlendirilmiş bir post-2011 SSNs Func_randomized_formatted_ssn bulur
    
  - Dokuz ardışık rakamlar (ddddddddd) biçimlendirilmemiş post-2011 SSNs Func_randomized_unformatted_ssn bulur
    
- **[Sağlama toplamı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Hayır, hiçbir sağlama yok 
    
- **[Tanımı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Bu tür hassas bilgiler algıladı emin %85 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer: 
    
  - [Func_ssn işlevi](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) bir desenle eşleşen içeriği bulur. 
    
  - [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) herhangi bir anahtar sözcük bulundu. Anahtar sözcük örnekleri içerir: *sosyal güvenlik, sosyal güvenlik #, Soc sn, SSN* . Örneğin, aşağıdaki örnek DLP SSN poliçesinin tetikleyecektir: **SSK: 489 36 8350**
    
Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi SSNs için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgi aramak için SSNs türleri](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

