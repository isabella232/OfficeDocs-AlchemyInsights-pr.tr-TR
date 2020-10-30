---
title: Intune Exchange şirket içi Bağlayıcısı
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808138"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange şirket içi Bağlayıcısı

Şirket içinde barındırılan Intune ile Exchange arasındaki bağlayıcıyı ayarlama ayrıntıları için aşağıdaki belgelere bakın:

[Microsoft Intune Azure 'da Intune şirket içi Exchange Connector 'ı ayarlama](https://docs.microsoft.com/intune/exchange-connector-install)

**SSS:**

S: Exchange Connector 'ı ayarlamaya çalışırken "Exchange Connector sürümü desteklenmiyor" gibi bir hata görüyorum. Neden olabilir?

A: kullandığınız hesap lisanslıdır; etkin bir Intune lisansı olmalıdır

S: birden çok Exchange Bağlayıcısı olabilir mi?

A: her bir Exchange kuruluşu için yalnızca bir Exchange Connector 'ı Intune kiracı başına ayarlayabilirsiniz. Bağlayıcı, çok sunuculu bir Exchange kuruluşunda yalnızca bir sunucuya yüklenebilir.

Ayrıca aynı kiracıda yapılandırılmış şirket içi hem de Exchange Online için yapılandırılmış bağlayıcılar olamaz.

S: bağlayıcının Exchange 'e bağlı olarak CAS dizisi kullanması mı istiyorsunuz?

A: CAS oluştururken desteklenen bir yapılandırma değildir. Yalnızca tek bir sunucu belirtilmeli ve bağlayıcı yapılandırma dosyasında bulunan ve

Program data\microsoft\şirket içi Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Aşağıdaki girdiyi bulun ```<ExchangeWebServiceURL />``` ve URL 'yi Exchange sunucusuyla değiştirin.

**Örnekteki**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ek sorun giderme için aşağıdaki belgelere bakın: [Intune şirket Içi Exchange bağlayıcısından sorun giderme](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Exchange Connector için ayrıntılı günlüğü etkinleştirme**

1. Exchange Connector izleme yapılandırma dosyasını düzenleme için açın.  
Dosya:% ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Örnekteki**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Aşağıdaki anahtarla TraceSourceLine bulun: OnPremisesExchangeConnectorService  
  
3. Bilgi etkinlik Izleme (varsayılan) ile ayrıntılı ActivityTracing  

**Örnekteki**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune Exchange hizmetini yeniden başlatma  
5. Sona erene kadar Intune portalında tam eşitleme ve XML 'i "bilgi ActivityTracing" olarak değiştirin ve Microsoft Intune Exchange hizmetini yeniden başlatın.  
6. Günlüklerin Konumu: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`