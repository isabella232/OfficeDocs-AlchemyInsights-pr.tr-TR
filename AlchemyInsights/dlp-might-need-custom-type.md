---
title: DLP özel bir tür gerekebilir
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932678"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP özel bir tür gerekebilir

**Önemli**: Birçok SharePoint Online ve OneDrive müşterisi, arka planda çalışan hizmete karşı iş açısından kritik uygulamalar çalıştırıyor. Bunlar arasında içerik geçişi, Veri Kaybıönleme (DLP) ve yedekleme çözümleri yer alır. Bu eşi görülmemiş zamanlarda, SharePoint Online ve OneDrive hizmetlerinin uzak çalışma senaryolarında hizmete her zamankinden daha fazla bağımlı olan kullanıcılarınız için son derece kullanılabilir ve güvenilir kalmasını sağlamak için adımlar atıyoruz.

Bu hedefi desteklemek için, hafta içi gündüz saatlerinde arka plan uygulamalarına (geçiş, DLP ve yedekleme çözümleri) daha sıkı azaltma limitleri uyguladık. Bu uygulamaların bu zamanlarda çok sınırlı bir iş artışı elde edeceğini bekleyebilirsiniz. Ancak, bölge için akşam ve hafta sonu saatlerinde, hizmet arka plan uygulamalarından gelen isteklerin önemli ölçüde daha yüksek hacimli işlemek için hazır olacaktır.

**DLP özel bir bilgi türü gerektirebilir**

Veri kaybıönleme (DLP) ilkesiyle, kuruluşunuzdaki hassas verileri tanımlayabilir ve koruyabilirsiniz. Bazı senaryolarda, kuruluşunuzun verilerini korumak için kendi **özel** duyarlı bilgi türünü oluşturmanız gerekebilir.

Örneğin, kuruluşunuzun çalışan kimliklerini veya orgunuza özgü bir biçimdeki diğer verileri tanımlaması ve koruması gerekebilir. Bu nedenle, daha fazla bilgi için aşağıdaki makalelere bakın.
  
 **Yerleşik duyarlı bilgi türünü özelleştirme**
  
Yerleşik bir hassas bilgi türü yalnızca birkaç değişiklikle ihtiyaçlarınızı karşılayacaksa, [yerleşik hassas bilgi türünü özelleştirebilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) Örneğin, anahtar kelimeler ekleyebilir veya kaldırabilir veya tarih veya adres gibi destekleyici kanıt ekleyebilir veya kaldırabilirsiniz.
  
 **Özel duyarlı bilgi türü oluşturma**
  
Ancak, farklı bir hassas bilgi türünü tamamen tanımlamanız ve korumanız gerekiyorsa, Güvenlik & Uyumluluk Merkezi'nin kullanıcı bilgi sinde [özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
  
**Güvenlik & Uyumluluk Merkezi PowerShell'de özel duyarlı bilgi türü oluşturma**

Son olarak, Kullanıcı Bira gereksinimi duyduğunuz tüm seçenekleri sağlamazsa, [Güvenlik & Uyumluluk Merkezi PowerShell'de özel bir bilgi türü oluşturabilirsiniz.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) Bir XML dosyasıyla başlayarak, kullanılabilir her seçeneği kullanabilirsiniz.
