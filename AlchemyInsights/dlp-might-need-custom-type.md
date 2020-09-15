---
title: DLP, özel bir türde olabilir
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
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712204"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP, özel bir türde olabilir

**Önemli**: Bu benzeri görünmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin kullanılabilirlik düzeyinin her zaman yüksek olmasını sağlamaya yönelik adımlar atıyoruz. Daha fazla bilgi için lütfen [SharePoint Online Geçici Özellik Değişiklikleri](https://aka.ms/ODSPAdjustments) sayfasını ziyaret edin.

**DLP, özel bilgi türü gerektirebilir**

Veri kaybı önleme (DLP) ilkesiyle, kuruluşunuzdaki hassas verileri tanımlayabilir ve koruyabilir. Bazı senaryolarda, kuruluşunuzun verilerini korumanız için kendi **özel** hassas bilgi türünüzün oluşturulması gerekebilir.

Örneğin, kuruluşunuzun kuruluşunuz için belirli biçimdeki çalışan kimliklerini veya diğer verileri belirleyip korumanız gerekebilir. Öyleyse, daha fazla bilgi için aşağıdaki makalelere bakın.
  
 **Yerleşik duyarlı bir bilgi türünü özelleştirme**
  
Yerleşik duyarlı bir bilgi türü yalnızca birkaç şeyle ihtiyaçlarınızı karşılıyorsa, [yerleşik duyarlı bir bilgi türünü özelleştirebilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Örneğin, anahtar sözcükleri ekleyebilir veya kaldırabilirsiniz ya da tarih veya adres gibi destekleyici bir kanıt ekleyebilir veya kaldırabilirsiniz.
  
 **Özel hassas bilgi türü oluşturma**
  
Ancak farklı türde duyarlı bilgileri tümüyle bulmanız ve korumanız gerekiyorsa, güvenlik & Uyumluluk Merkezi Kullanıcı arabiriminde [özel bir hassas bilgi türü oluşturabilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) .
  
**Güvenlik & Uyumluluk Merkezi PowerShell 'de özel hassas bir bilgi türü oluşturma**

Son olarak, Kullanıcı arabirimi ihtiyaç duyacağınız tüm seçenekleri sağlamıyorsa, [güvenlik & Uyumluluk Merkezi PowerShell 'de özel bir hassas bilgi türü oluşturabilirsiniz](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Bir XML dosyasıyla başlayarak, sağlanan her seçeneği kullanabilirsiniz.
