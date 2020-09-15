---
title: ABD/INGILTERE Passport numarası için DLP kuralı çalışmıyor
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679244"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP-US/INGILTERE Passport numaralarıyla ilgili sorunlar

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**ABD/INGILTERE Passport numaralarıyla DLP sorunları**

O365 'de DLP duyarlı bir bilgi türü kullanırken, **ABD/İngiltere Passport numarası** içeren Içerik Için **veri kaybı önleme (DLP)** sorunlarıyla ilgili sorun mu yaşıyorsunuz? Bu durumda, içeriğinizin değerlendirilme sırasında hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun.
  
Örneğin, %75 güvenilirlik düzeyiyle yapılandırılmış **US/İngiltere Passport numarası** ilkesi için, aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dokuz basamak

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Art arda dokuz basamak

- **[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, sağlama toplamı yok

- **[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %75.

  - İşlev Func_usa_uk_passport desenle eşleşen içeriği bulur.

  - Keyword_passport 'dan bir anahtar sözcük bulundu.

    Örneğin, aşağıdaki örnek **ABD/İngiltere Passport numarası** ilkesi için tetikleyecektir: ABD pasaport numarası 123456789

İçeriğiniz için ABD/INGILTERE Passport numarasının gerekli olduğu hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne bakın: [duyarlı bilgi türleri IÇIN ABD/Ingiltere Passport numarasını](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) görüntüleme
  
Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  