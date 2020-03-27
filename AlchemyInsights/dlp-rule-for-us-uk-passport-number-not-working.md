---
title: ABD/İngiltere Pasaport Numarası çalışmıyor için DLP kuralı
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977126"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP ile ilgili sorunlar - ABD/İngiltere pasaport numaraları

**Önemli**: Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin yüksek oranda kullanılabilir kalmasını sağlamak için adımlar atıyoruz – Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Ayarlamaları'nı](https://aka.ms/ODSPAdjustments) ziyaret edin.

**ABD/İngiltere pasaport numaraları ile DLP sorunları**

O365'te DLP hassas bilgi türünü kullanırken **ABD/İngiltere pasaport numarası** içeren içerik için çalışmayan Veri Kaybı Önleme **(DLP)** ile ilgili sorunlar mı yaşıyorsunuz? Bu nedenle, içeriğinizin DLP ilkesinin değerlendirildiğinde aradığı bilgiler için gerekli bilgileri içerdiğinden emin olun.
  
Örneğin, %75 güven düzeyine sahip yapılandırılmış bir **ABD/Birleşik Krallık pasaport numarası** politikası için aşağıdakiler değerlendirilir ve kuralın tetiklemesi için algılanmalıdır
  
- **[Biçimlendirme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dokuz basamak

- **[Desen:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Art arda dokuz basamak

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Hayır, Checksum diye bir şey yok.

- **[Tanım:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Bir DLP ilkesi, 300 karaktere yakın bir mesafede bu tür hassas bilgileri algılayıştıracağından %75 emindir:

  - İşlev Func_usa_uk_passport desenle eşleşen içeriği bulur.

  - Keyword_passport'dan bir anahtar kelime bulunur.

    Örneğin, aşağıdaki örnek **ABD/İngiltere pasaport numarası** politikası için tetikleyici olacaktır: ABD Pasaport numarası 123456789

İçeriğiniz için abd/Birleşik Krallık Pasaport Numarasının algılanması için gerekenler hakkında daha fazla bilgi için bu makaledeki aşağıdaki bölüme bakın: [Hassas Bilgi Türleri ABD/Birleşik Krallık Pasaport Numarası için ne arar](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Farklı bir yerleşik duyarlı bilgi türünü kullanarak, diğer türler için nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: [Hassas Bilgi Türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  