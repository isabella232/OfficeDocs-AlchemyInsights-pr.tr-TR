---
title: Kredi kartı numarası için DLP kuralı çalışmıyor
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679461"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Kredi kartı numaralarıyla ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**Kredi kartı numaralarıyla ilgili DLP sorunları**

O365 'de DLP duyarlı bir bilgi türü kullanırken, **kredi kartı numarası** içeren Içerik Için **veri kaybı önleme (DLP)** sorunlarıyla karşılaşmıyorsunuz mı? Bu durumda, içeriğinizin değerlendirilme sırasında DLP ilkesini tetiklemek için gerekli bilgileri içerdiğinden emin olun. Örneğin, %85 güvenilirlik düzeyiyle yapılandırılmış bir **kredi kartı ilkesinde** , aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir:
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** biçimlendirilebilen veya biçimlendirilmemiş (dddddddddddddddd) 16 basamak.

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Visa, MasterCard, keşif kartı, JCB, Amerikan Express, hediye kartları ve Diner kartları dahil tüm dünya genelindeki tüm önemli markalardan kartlar algılayan çok karmaşık ve güçlü bir düzen.

- **[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Evet, Luhn sağlaması

- **[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %85.

  - İşlev Func_credit_card desenle eşleşen içeriği bulur.

  - Aşağıdakilerden biri doğrudur:

  - Keyword_cc_verification 'dan bir anahtar sözcük bulundu.

  - Keyword_cc_name 'dan bir anahtar sözcük bulundu

  - İşlev Func_expiration_date, sağ tarih biçiminde bir tarih bulur.

  - Sağlama toplamı geçişlerinde

    Örneğin, aşağıdaki örnek bir DLP kredi kartı numarası Ilkesi için tetikleyecektir:

  - Visa: 4485 3647 3952 7352
  
  - Süre sonu: 2/2009

İçeriğiniz için bir **kredi kartı numarasının** gerekli olması gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [kredi kartı # Için hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  