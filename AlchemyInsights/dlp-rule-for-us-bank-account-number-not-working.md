---
title: ABD Banka Hesap Numarası için DLP kuralı çalışmıyor
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005038"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ABD banka hesap numaralarıyla ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**ABD banka hesap numaralarıyla ilgili DLP sorunları**

O365'te DLP'ye duyarlı bir bilgi  türü kullanırken, Veri Kaybı Önleme **(DLP)** önleme ile ilgili sorunlarınız mı var? Öyleyse, içeriğinizin, DLP ilkesi değerlendirilirken ne zaman aray olduğuna ilişkin gerekli bilgileri içerdiğine emin olun.
  
Örneğin, %85 güven düzeyiyle yapılandırılmış ABD Banka Hesap Numarası ilkesi için aşağıdakiler değerlendirilir ve kuralın tetikley algısı gerekir: 
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 basamak

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 art arda basamaklar.

- **[DenetimUmum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, Checksum yok

- **[Tanım:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP ilkesi, bu tür hassas bilgilerin 300 karakter yakınlıkta algılandığından %75 oranında emindir:

  - Normal ifade Regex_usa_bank_account_number desene eşleşen içeriği bulur

  - Anahtar sözcük Keyword_usa_Bank_Account bulunur.

    Örneğin, aşağıdaki örnek ABD Banka Hesap Numarası ilkesi için **tetiklenir:** Hesap Denetimi 78344011

İçeriğiniz için ABD Banka  Hesabı Numarasının algılandığında nelerin gerekli olduğu hakkında daha fazla bilgi için, bu makaledeki şu bölüme bakın: Hassas Bilgi Türleri ABD Banka Hesap Numarası'nın [nasıl görünüyor?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Farklı bir yerleşik hassas bilgi türü kullanarak, diğer türlerde nelerin gerekli olduğu hakkında bilgi için aşağıdaki makaleye bakın: Hassas Bilgi [Türleri'nin neleri araması](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  