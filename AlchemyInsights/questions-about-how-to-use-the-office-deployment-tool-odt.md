---
title: Office dağıtım aracı 'nı (ODT) kullanma hakkında sorular
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774911"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office dağıtım aracı 'nı (ODT) kullanma hakkında sorular

Office dağıtım aracı 'nı [Microsoft Yükleme Merkezi](https://go.microsoft.com/fwlink/p/?LinkID=626065)'nden yükleyin.
  
Dosyayı indirdikten sonra, Office dağıtım Aracı yürütülebilir (setup.exe) ve örnek yapılandırma dosyası (configuration.xml) içeren kendiliğinden ayıklanan yürütülebilir dosyayı çalıştırabilirsiniz.
  
 **Kurumsal Ürünler için Microsoft 365 uygulamalarını istemci bilgisayarlardan dışlamak veya kaldırmak için:**
  
Kuruluş için Microsoft 365 uygulamalarını yüklerken belirli ürünleri dışlayabilirsiniz. Bunu yapmak için, Office 'i ODT ile yükleme adımlarını izleyin, ancak yapılandırma dosyanıza ExcludeApp öğesini ekleyin. Örneğin, bu yapılandırma dosyası Publisher dışında kurumsal ürünler için Microsoft 365 uygulamalarını yükler:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office dağıtım aracına genel bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

