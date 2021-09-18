---
title: DLP'ye özel bir tür gerekiyor olabilir
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446711"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP'ye özel bir tür gerekiyor olabilir

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**DLP için özel bir bilgi türü gerekli olabilir**

Veri kaybını önleme (DLP) ilkesiyle, kuruluşta hassas verileri tanımlayabilir ve koruyabilirsiniz. Bazı senaryolarda, kendi özel hassas bilgi türlerinizi oluşturmak ve kurum verilerinizi korumak için ihtiyacınız olabilir. Daha fazla bilgi için [bkz. Hassas bilgi türleri ve Hassas](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) bilgi türü varlık [tanımları hakkında bilgi.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Özel hassas bilgi türleri ve ilkeleri oluşturma hakkında daha fazla bilgi için bkz: 

**Yerleşik hassas bilgi türünü özelleştirme**

Yerleşik bir hassas bilgi türü yalnızca birkaç düzeltmeyle gereksinimlerinizi karşılayacaksa, [bkz. Yerleşik](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)hassas bilgi türünü özelleştirme . Örneğin, anahtar sözcükler ekleyebilir veya kaldırabilir ya da tarih veya adres gibi destekleyen kanıt ekleyebilir veya kaldırabilirsiniz.

**Özel hassas bilgi türü oluşturma**

Ancak, farklı türde hassas bilgileri bir bir şekilde tanımlamaya ve korumaya gerek varsa, çalışma sayfalarında özel bir hassas bilgi Microsoft 365 uyumluluk merkezi. Daha fazla bilgi için [bkz. Özel hassas bilgi türleriyle çalışmaya başlama.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Güvenlik ve Uyumluluk Merkezi PowerShell'de özel & bilgi türü oluşturma**

Son olarak, kullanıcı arabirimi size gereken tüm seçenekleri sağlayamasa da, Güvenlik ve Uyumluluk Merkezi PowerShell'de özel & bilgi türü oluşturabilirsiniz. XML dosyasıyla başlayarak, kullanılabilir tüm seçenekleri kullanabilirsiniz. Daha fazla bilgi için [bkz. PowerShell kullanarak özel duyarlı bilgi türü oluşturma.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

İlk olarak test modunda ilkenizi test etmek için [bkz. İlkeyi test](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) modunda uygulama ve DLP ilkesi [oluşturma, sınama ve ayarlama.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 