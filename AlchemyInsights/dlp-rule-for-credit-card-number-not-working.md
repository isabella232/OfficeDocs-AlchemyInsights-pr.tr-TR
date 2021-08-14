---
title: Kredi Kartı Numarası için DLP Kuralı çalışmıyor
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005110"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Kredi kartı numaralarıyla ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**Kredi kartı numaralarıyla ilgili DLP sorunları**

O365'te DLP'ye duyarlı bir bilgi  türü kullanılırken, Veri Kaybı Önleme **(DLP) önleme (DLP)** içeriğinde sorun mu oluyor? Varsa, içeriğinizin, DLP ilkesi değerlendirilirken tetiklenirken gereken bilgileri içerdiğine emin olun. Örneğin, %85 güven düzeyiyle yapılandırılmış bir Kredi Kartı ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklen değerlendirmesine neden olması gerekir: 
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** Biçimlendirilmiş veya biçimlendirilmemiş (ddddd) 16 basamak ve Luhn testini geçmeleri gerekir.

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Visa, MasterCard, Discover Card, JCB, American Express, hediye kartları ve kartvizitler gibi dünya çapındaki tüm önemli markalardan kartları algılayan çok karmaşık ve güçlü bir desen.

- **[DenetimUmum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Evet, Luhn checksum

- **[Tanım:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP ilkesi, 300 karakter yakınlıkta olduğu durumda bu tür hassas bilgilerin algılandığından %85 emindir:

  - İşlev Func_credit_card desene eşleşen içeriği bulur.

  - Aşağıdakilerden biri doğrudur:

  - Farklı bir Keyword_cc_verification anahtar sözcük bulunur.

  - Bir başka Keyword_cc_name anahtar sözcük bulunur

  - İşlev Func_expiration_date tarih biçimindeki bir tarihi bulur.

  - Denetimli denetimler geçer

    Örneğin, aşağıdaki örnek DLP Kredi Kartı Numarası İlkesini tetikler:

  - Visa: 4485 3647 3952 7352
  
  - Son kullanma tarihi: 2/2009

İçeriğiniz için Kredi Kartı  Numarasının algılandığında nelerin gerekli olduğu hakkında daha fazla bilgi için, bu makalenin şu bölümüne bakın: Hassas Bilgi Türleri Kredi Kartı# için nelerin [görünüyor?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Farklı bir yerleşik hassas bilgi türü kullanarak, diğer türlerde nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: Hassas Bilgi [Türleri'nin neleri araması](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  