---
title: ABD Banka Hesap Numarası çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932570"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ABD banka hesap numaraları ile DLP sorunları

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

**ABD banka hesap numaraları ile DLP sorunları**

O365'te DLP'ye duyarlı bilgi türünü kullanırken **ABD Banka Hesap Numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz? Bu nedenle, içeriğinizin DLP ilkesinin değerlendirildiğinde aradığı bilgiler için gerekli bilgileri içerdiğinden emin olun.
  
Örneğin, %85 güven düzeyiyle yapılandırılan bir **ABD Banka Hesap Numarası** ilkesi için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 basamak

- **[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ardışık basamak.

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, Checksum diye bir şey yok.

- **[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %75 emindir:

  - Normal ifade Regex_usa_bank_account_number desenle eşleşen içeriği bulur

  - Keyword_usa_Bank_Account'dan bir anahtar kelime bulunur.

    Örneğin, AŞAĞıDAKI örnek **ABD Banka Hesap Numarası** politikası için tetikleyeceği gibi: Çek Hesabı 78344011

İçeriğiniz için bir ABD **Banka Hesap Numarasının** algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri ABD Banka Hesap Numarası için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  