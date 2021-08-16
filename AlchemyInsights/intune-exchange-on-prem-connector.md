---
title: Intune Exchange bağlayıcısı
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013984"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange bağlayıcısı

Intune ile şirket içinde barındırılan Exchange bağlayıcıyı ayarlamanın ayrıntıları için lütfen aşağıdaki belgelere bakın:

[Azure'da Intune şirket içi Exchange bağlayıcısı Microsoft Intune ayarlama](https://docs.microsoft.com/intune/exchange-connector-install)

**SSS:**

S: Yeni bağlayıcıyı ayarlamaya çalışırken "Exchange Bağlayıcısı sürümü desteklenmiyor" gibi bir Exchange görüyorum. Bunun nedeni nedir?

A: Kullanmakta olduğu hesap uygun şekilde lisanslandı - Etkin bir Intune lisansına sahip olması gerekir

S: Birden fazla bağlayıcının birden Exchange olabilir mi?

Y: Her kuruluş için Intune Exchange tek bir bağlayıcı Exchange ayar). Bağlayıcı yalnızca çok sunuculu bir Exchange kuruluşunda tek bir sunucuya yüklenebilirsiniz.

Ayrıca, aynı kiracıda hem şirket içi Exchange hem de Exchange Online için yapılandırılmış bağlayıcınız olamaz.

S: Bağlayıcı, diziye bağlantı olarak CAS dizisini Exchange?

A: CAS dizisi belirtmek, bağlayıcı kurulumunda desteklenen bir yapılandırma değildir. Yalnızca tek bir sunucu belirtilmelidir ve bu sunucuda bulunan bağlayıcı yapılandırma dosyasında sabit kodlandırilmelidir:

program data\microsoft\microsoft Intune şirket içi Exchange bağlayıcısı\ OnpremiseExchangeConnectorServiceConfiguration.xml

Aşağıdaki girdiyi bulun ```<ExchangeWebServiceURL />``` ve URL'yi Exchange sunucusuyla değiştirin.

**Örnek:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ek sorun giderme için lütfen aşağıdaki belgelere bakın: [Intune şirket içi](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) bağlayıcısı Exchange giderme

**Exchange bağlayıcısı için Ayrıntılı Exchange etkinleştirme**

1. Düzenlemek için Exchange İzleme yapılandırma dosyasını açın.  
Dosya : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Örnek:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Aşağıdaki anahtarı kullanarak TraceSourceLine'ı bulun: OnPremisesExchangeConnectorService  
  
3. SourceLevel düğüm değerini Bilgi EtkinliğiTracing'den (varsayılan) Verbose ActivityTracing olarak değiştirme  

**Örneğin:**
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
4. Microsoft Intune Exchange Hizmetini yeniden başlatma  
5. Intune Portalında tam eşitleme bitene kadar bekleyin ve sonra XML'yi yeniden "Bilgi EtkinliğiNuma" olarak yeniden başlatın ve Microsoft Intune Exchange başlatın.  
6. Günlüklerin konumu: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`