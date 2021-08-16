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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030814"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP'ye özel bir tür gerekiyor olabilir

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**DLP için özel bir bilgi türü gerekli olabilir**

Veri kaybını önleme (DLP) ilkesiyle, kuruluşta hassas verileri tanımlayabilir ve koruyabilirsiniz. Bazı senaryolarda, kendi özel hassas  bilgi türlerinizi oluşturmak ve kurum verilerinizi korumak için ihtiyacınız olabilir.

Örneğin, kuruma özgü çalışan kimliklerini veya diğer verileri belirli bir biçimde tanımlaması ve korumaları gerekiyor olabilir. Öyleyse, daha fazla bilgi için aşağıdaki makalelere bakın.
  
 **Yerleşik hassas bilgi türünü özelleştirme**
  
Yerleşik bir hassas bilgi türü yalnızca birkaç düzeltmeyle gereksinimlerinizi karşılayacaksa, yerleşik bir hassas bilgi [türünü özelleştirebilirsiniz.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Örneğin, anahtar sözcükler ekleyebilir veya kaldırabilir ya da tarih veya adres gibi destekleyen kanıt ekleyebilir veya kaldırabilirsiniz.
  
 **Özel hassas bilgi türü oluşturma**
  
Ancak farklı türde hassas bilgileri bir bir şekilde tanımlamaya [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) ve korumaya gerek olursa, Güvenlik ve Uyumluluk Merkezi'nin kullanıcı arabiriminde özel bir hassas bilgi & oluşturabilirsiniz.
  
**Güvenlik ve Uyumluluk Merkezi PowerShell'de özel & bilgi türü oluşturma**

Son olarak, kullanıcı arabirimi size gereken tüm seçenekleri sağlayamasa da, Güvenlik ve Uyumluluk Merkezi PowerShell'de özel & [bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) XML dosyasıyla başlayarak, kullanılabilen tüm seçenekleri kullanabilirsiniz.
