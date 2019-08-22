---
title: Kredi kartı numarası çalışmıyor DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529975"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Kredi kartı numaraları DLP sorunları

**Veri kaybını önleme (DLP)** içinde O365 DLP hassas bilgi türünü kullanırken, bir **Kredi kartı numarası** içeren içerik için çalışmıyor sorun yaşıyorsunuz? Öyleyse, içeriğinizi tetiklemek için gerekli bilgileri içerdiğinden emin olun Bunu değerlendirildiğinde DLP ilkesi. Örneğin, % 85 bir güvenirlik düzeyiyle yapılandırılmış bir **Kredi kartı İlkesi** , aşağıdaki değerlendirilir ve kural tetiklemek algılandı:
  
- **[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** hangi biçimlendirilebilir 16 basamak veya biçimlendirilmemiş (dddddddddddddddd) ve Luhn sınamasından geçmesi gerekir.

- **[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa, MasterCard, keşfedin kartı, JCB, American Express, hediye kartları ve diner kartları da dahil olmak üzere dünya çapında, tüm önemli markalar kartlardan algılar çok karmaşık ve güçlü deseni.

- **[Sağlama toplamı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Evet, Luhn sağlama

- **[Tanımı:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Bu tür hassas bilgiler algıladı emin %85 DLP ilkedir 300 karakterden oluşan bir yakınlık içinde Eğer:

  - Func_credit_card işlevi bir desenle eşleşen içeriği bulur.

  - Aşağıdakilerden biri doğrudur:

  - Keyword_cc_verification herhangi bir anahtar sözcük bulundu.

  - Keyword_cc_name herhangi bir anahtar sözcük bulunamadı

  - Func_expiration_date işlevi doğru tarih biçimindeki bir tarihi bulur.

  - Sağlama toplamı geçirir

    Örneğin, aşağıdaki örnek DLP kredi kartı numarası poliçesinin tetikler:

  - Visa: 4485 3647 3952 7352
  
  - Son kullanma tarihi: 2/2009

Bu makalede aşağıdaki bölümde içeriğiniz için algılanabilmesi bir **Kredi kartı numarası** için gerekli olan daha fazla bilgi için bkz: [Ne hassas bilgi aramak için kredi kartı # türleri](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Bir başka yerleşik hassas bilgi türünü kullanarak aşağıdaki bilgiler makalesine bakın diğer türleri için gerekli olan temel: [ne hassas bilgi türlerini aramak](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  