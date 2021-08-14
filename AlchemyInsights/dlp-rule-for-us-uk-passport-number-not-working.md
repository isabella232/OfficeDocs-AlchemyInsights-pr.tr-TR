---
title: ABD/İngiltere Pasaport Numarası için DLP kuralı çalışmıyor
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004966"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP - ABD/İngiltere pasaport numaralarıyla ilgili sorunlar

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**ABD/İngiltere pasaport numaralarıyla ilgili DLP sorunları**

O365'te DLP hassas bilgi türü kullanırken, Veri Kaybı Önleme **(DLP) önleme (DLP)** numarası içeren içerikte **ABD/İngiltere** pasaportunu içeren içerikte sorun mu alısınız? Öyleyse, içeriğinizin, DLP ilkesi değerlendirilirken ne zaman aray olduğuna ilişkin gerekli bilgileri içerdiğine emin olun.
  
Örneğin, %75 güven düzeyinde yapılandırılan **ABD/İngiltere** pasaport ilkesinde, aşağıdakiler değerlendirilir ve kuralın tetikley algısı gerekir
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dokuz rakam

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Art arda dokuz basamak

- **[DenetimUmum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, Checksum yok

- **[Tanım:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP ilkesi, bu tür hassas bilgilerin 300 karakter yakınlıkta algılandığından %75 oranında emindir:

  - İşlev Func_usa_uk_passport desene eşleşen içeriği bulur.

  - Anahtar sözcük Keyword_passport bulunur.

    Örneğin, aşağıdaki örnek, **ABD/İngiltere** pasaport numarası ilkesi için tetik tetikler: ABD Pasaport 123456789

İçeriğiniz için ABD/Birleşik Krallık Pasaport Numarası algılandığında nelerin gerekli olduğu hakkında daha fazla bilgi için, bu makaledeki şu bölüme bakın: Hassas Bilgi Türleri [ABD/İngiltere](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) Pasaport Numarası'nın nasıl görünüyor?
  
Farklı bir yerleşik hassas bilgi türü kullanarak, diğer türlerde nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: Hassas Bilgi [Türleri'nin neleri araması](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  