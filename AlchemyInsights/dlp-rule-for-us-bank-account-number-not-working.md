---
title: DLP kural numaralı BİZE banka hesabı çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404298"
---
**Veri kaybını önleme (DLP)** içinde O365 DLP hassas bilgi türünü kullanırken, bir **ABD banka hesap numarasını** içeren içerik için çalışmıyor sorun yaşıyorsunuz? Öyleyse, emin olun, içeriğinizi onu değerlendirildiğinde DLP İlkesi aramak gerekli bilgileri içerir. 
  
Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir **ABD banka hesap numarası** ilke için aşağıdaki değerlendirilir ve kural tetiklemek algılandı: 
  
- **[Biçimi:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 basamak 
    
- **[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ardışık rakamlar. 
    
- **[Sağlama toplamı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, hiçbir sağlama yok 
    
- **[Tanımı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Bu tür hassas bilgiler algıladı emin % 75 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer: 
    
  - Desenle eşleşen içerik Regex_usa_bank_account_number normal ifade bulur
    
  - Keyword_usa_Bank_Account herhangi bir anahtar sözcük bulundu.
    
    Örneğin, aşağıdaki örnek **ABD banka hesap numarası** poliçesinin tetikleyecektir: Çek Hesabı 78344011 
    
Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi **ABD banka hesap numarası** için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgileri ABD banka hesap numarası için arama türleri](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

