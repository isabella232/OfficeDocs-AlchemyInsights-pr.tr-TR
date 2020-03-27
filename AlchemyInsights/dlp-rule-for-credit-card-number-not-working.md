---
title: Kredi Kartı Numarası çalışmıyor için DLP Kuralı
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977218"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Kredi kartı numaraları ile DLP sorunları

**Önemli**: Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin yüksek oranda kullanılabilir kalmasını sağlamak için adımlar atıyoruz – Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Ayarlamaları'nı](https://aka.ms/ODSPAdjustments) ziyaret edin.

**Kredi kartı numaraları ile DLP sorunları**

O365'te DLP duyarlı bilgi türü kullanırken **Kredi Kartı Numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz? Bu nedenle, içeriğinizin DLP ilkesini tetiklemek için gerekli bilgileri içerdiğinden emin olun. Örneğin, %85 güven düzeyiyle yapılandırılan bir **Kredi Kartı politikası** için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:
  
- **[Biçim:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** Biçimlendirilebilir veya biçimlendirilmemiş (dddddddddddddddd) ve Luhn testini geçmek zorundadır 16 basamak.

- **[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa, MasterCard, Discover Card, JCB, American Express, hediye kartları ve yemek kartları dahil olmak üzere dünya çapındaki tüm büyük markaların kartlarını algılayan çok karmaşık ve sağlam desen.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Evet, Luhn çekleri.

- **[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %85 emindir:

  - İşlev Func_credit_card desenle eşleşen içeriği bulur.

  - Aşağıdakilerden biri doğrudur:

  - Keyword_cc_verification'dan bir anahtar kelime bulunur.

  - Keyword_cc_name'dan bir anahtar kelime bulundu

  - İşlev Func_expiration_date doğru tarih biçiminde bir tarih bulur.

  - Checksum geçer

    Örneğin, aşağıdaki örnek bir DLP Kredi Kartı Numarası Politikası için tetikler:

  - Vize: 4485 3647 3952 7352
  
  - Bitiş Tarihi: 2/2009

İçeriğiniz için kredi kartı **numarasının** algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri Kredi Kartı için ne arar#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  