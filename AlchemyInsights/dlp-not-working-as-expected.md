---
title: DLP beklendiği gibi çalışmıyor
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079722"
---
# <a name="dlp-not-working-as-expected"></a>DLP beklendiği gibi çalışmıyor

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

 **DLP'i ayarlama**

Bu çalışmalarda Veri **Kaybı Önleme (DLP)** ile ilgili sorunlar Office 365 çalışmaıyor musunuz? Bu varsa, **DLP** ilkenizin doğru ayarlanmış olduğundan ve verilerinizde **DLP** ilkesi değerlendirilirken arayacakları içeriği olduğundan emin olun.
  
DLP ilkeleri, kuruluşta hassas bilgileri tanımlamanıza ve korumanıza olanak sağlar. DLP ilkelerinin kurulumu için buradaki bilgileri [kullanın.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **DLP ilkeleri nasıl görünüyor?**
  
Güvenlik ve **Uyumluluk merkezlerindeki** yerleşik hassas bilgi türleri kullanılırken, DLP ilkeleri bu hassas türleri algılarken belirli desenleri ve öğeleri aramaz.
  
- **Yerleşik Hassas Bilgi Türleri**

    Yerleşik Hassas türler ve DLP ilkesi Hassas türü algı olduğunda nasıl bir DLP ilkesi araması hakkında bilgi için bkz. Hassas bilgi [türleri ne için arama yaptı.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Özel Hassas Bilgi Türleri**

    Özel hassas bilgi türleri oluşturma üzerinde çalışıyorsanız, özel duyarlı tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: Özel duyarlı [bilgi türü oluşturma.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP ilkesi sınama**

Verilerinizi yerleşik veya özel bir hassas bilgi türüyle test etmek için Sınıflandırmalar Duyarlı bilgi türleri altındaki **Test** **türü**  >  **seçeneğini kullanın.** Daha fazla bilgi için [bkz. Özel hassas bilgi türlerini test edin.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raporlar**
  
- DLP Raporları ile hassas [veri içgörüleri elde edin.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Olay Raporu ile olayın belirli [ayrıntılarına bakın.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
