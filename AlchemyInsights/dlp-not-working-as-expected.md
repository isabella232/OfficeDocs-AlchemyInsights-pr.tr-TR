---
title: DLP beklendiği gibi çalışmıyor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932642"
---
# <a name="dlp-not-working-as-expected"></a>DLP beklendiği gibi çalışmıyor

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

 **DLP'nin ayarlanması**

Office 365'te **veri kaybının önlenmesi (DLP)** ile ilgili sorunlar mı yaşıyorsunuz? Bu nedenle, **DLP ilkenizin** doğru şekilde ayarlandığınızdan ve verilerinizin **DLP ilkesinin** değerlendirilirken aradığı şeyi içerdiğinden emin olun.
  
DLP ilkeleri, kuruluşunuzdaki hassas bilgileri tanımlamanıza ve korumanıza olanak tanır. DLP ilkelerini kurmak için [buradaki](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)bilgileri kullanın.
  
 **DLP ilkeleri ne leri arar**
  
Office 365 Güvenlik ve Uyumluluk merkezinde **yerleşik hassas bilgi türlerini** kullanırken, DLP ilkeleri bu hassas türleri algılarken belirli desenleri ve öğeleri arar.
  
- **Yerleşik Hassas Bilgi Türleri**

    Yerleşik Hassas türleri ve Bir DLP ilkesinin Hassas türü algılarken ne aradığı hakkında bilgi için bkz: [Hassas bilgi türlerinin aradığı](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)şey.

- **Özel Hassas Bilgi Türleri**

    Özel duyarlı bilgi türleri oluşturmaya çalışıyorsanız, özel duyarlı bir tür oluşturma hakkında bilgi için aşağıdaki makaleyi kullanın: [Özel duyarlı bilgi türü oluşturun.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)

**Bir DLP ilkesini test edin**

Verilerinizi yerleşik veya özel olarak duyarlı bilgi türüyle **sınamak** > için, Sınıflandırmalara**Duyarlı bilgi türleri**altında Test **türü** seçeneğini kullanın. Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)

 **Raporlar**
  
- [DLP Raporları](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) ile hassas veri öngörüleri alın.

- [Olay Raporu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)ile olayın belirli ayrıntılarını görün.
