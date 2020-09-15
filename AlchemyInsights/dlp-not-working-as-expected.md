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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679713"
---
# <a name="dlp-not-working-as-expected"></a>DLP beklendiği gibi çalışmıyor

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

 **DLP 'yi ayarlama**

Office 365 'de **veri kaybı önleme (DLP)** ile ilgili sorun mu yaşıyorsunuz? Öyleyse, **DLP ilkenizin** doğru ayarlandığından ve verilerinizde **DLP ilkesinin** değerlendirilme sırasında hangi özelliklere sahip olduğundan emin olun.
  
DLP ilkeleri kuruluşunuzdaki hassas bilgileri tanımlamanıza ve korumanızı sağlar. DLP ilkelerini ayarlamak için [buradaki](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)bilgileri kullanın.
  
 **Hangi DLP politikalarını arar**
  
Güvenlik ve uyumluluk merkezlerinde **yerleşik duyarlı bilgi türlerini** KULLANıRKEN, DLP ilkeleri bu hassas türleri algılayarak belirli desenleri ve öğeleri arar.
  
- **Yerleşik duyarlı bilgi türleri**

    Yerleşik duyarlı türler [ve duyarlı türü](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)algılayarak bir DLP İlkesi görünme hakkında bilgi için bkz.

- **Özel hassas bilgi türleri**

    Özel hassas bilgi türleri oluşturmaya çalışıyorsanız, özel hassas bir tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: [özel hassas bilgi türü oluşturma](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**DLP ilkesini sınama**

Verilerinizi yerleşik veya özel bir hassas bilgi türüyle sınamak için **Classifications**hassas bilgi türleri 'nin altındaki **test türü** seçeneğini kullanın  >  **Sensitive info types**. Daha fazla bilgi [için bkz.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raporlar**
  
- [DLP raporlarıyla](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports) hassas veri öngörülerini edinin.

- Olay [raporu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)ile olayın belirli ayrıntılarını görün.
