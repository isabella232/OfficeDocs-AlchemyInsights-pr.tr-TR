---
title: DLP kuralı ABD / İngiltere Pasaport numarası çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318530"
---
**Veri kaybını önleme (DLP)** içerik içeren için çalışmıyor ile sorunlarınız bir **ABD / İngiltere Pasaport numarası** içinde O365 DLP hassas bilgi türünü kullanırken? Öyleyse, emin olun, içeriğinizi onu değerlendirildiğinde DLP İlkesi aramak gerekli bilgileri içerir. 
  
Örneğin, bir **ABD / İngiltere Pasaport numarası** güvenirlik düzeyini % 75 ile yapılandırılan ilke, aşağıdaki değerlendirilir ve kural tetiklemek algılandı 
  
- **[Biçimi:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dokuz basamak 
    
- **[Desen:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Art arda dokuz basamak 
    
- **[Sağlama toplamı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, hiçbir sağlama yok 
    
- **[Tanımı:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Bu tür hassas bilgiler algıladı emin % 75 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer: 
    
  - Func_usa_uk_passport işlevi bir desenle eşleşen içeriği bulur.
    
  - Keyword_passport herhangi bir anahtar sözcük bulundu.
    
    Örneğin, aşağıdaki örnek için tetikleyecektir **ABD / İngiltere Pasaport numarası** İlkesi: 123456789 ABD Pasaport numarası 
    
Hakkında daha fazla bilgi için bir US gereklidir / İngiltere Pasaport numarası içeriğiniz için algılanabilmesi için bu makaledeki aşağıdaki bölümüne bakın: [ne hassas bilgi türlerini arayın, ABD / İngiltere Pasaport numarası](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

