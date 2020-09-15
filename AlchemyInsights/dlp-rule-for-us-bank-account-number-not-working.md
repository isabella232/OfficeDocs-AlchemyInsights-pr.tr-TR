---
title: ABD banka hesap numarası için DLP kuralı çalışmıyor
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679316"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>ABD banka hesap numaralarıyla ilgili DLP sorunları

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**ABD banka hesap numaralarıyla ilgili DLP sorunları**

O365 'de DLP duyarlı bir bilgi türü kullanırken, **ABD banka hesap numarası içeren bir ABD banka hesap numarası** içeren içerik Için çalışmayan **veri kaybı önleme (DLP)** sorunlarıyla karşılaşıyor musunuz? Bu durumda, içeriğinizin değerlendirilme sırasında hangi özelliklere sahip olduğuna ilişkin gerekli bilgileri içerdiğinden emin olun.
  
Örneğin, %85 güvenilirlik düzeyiyle yapılandırılmış **US banka hesap numarası** ilkesinde, aşağıdakiler değerlendirilir ve kuralın tetiklenmesi için algılanabilmesi gerekir:
  
- **[Biçim:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 basamak

- **[Desen:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ardışık basamaklar.

- **[Sağlama toplamı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Hayır, sağlama toplamı yok

- **[Tanımı:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP İlkesi, 300 karakterlerinin bir yakınlığı ile bu tür hassas bilgileri algıladığı için %75.

  - Normal ifade Regex_usa_bank_account_number desenle eşleşen içeriği bulur

  - Keyword_usa_Bank_Account 'dan bir anahtar sözcük bulundu.

    Örneğin, aşağıdaki örnek **ABD banka hesap numarası** ilkesini tetikleyecektir: hesap 78344011

İçeriğiniz için bir **ABD banka hesap numarasının** gerekli olması gerekenler hakkında daha fazla bilgi için, bu makalenin aşağıdaki bölümüne BAKıN: [ABD banka hesap numarası Için hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Farklı yerleşik duyarlı bir bilgi türü kullanarak, diğer türler için gerekenler hakkında bilgi için aşağıdaki makaleye bakın: [hassas bilgi türleri](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  