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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932463"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Kredi kartı numaraları ile DLP sorunları

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

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
  