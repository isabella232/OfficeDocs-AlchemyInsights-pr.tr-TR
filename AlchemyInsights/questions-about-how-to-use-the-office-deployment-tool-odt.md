---
title: Office Dağıtım Aracı'nı (ODT) kullanma hakkında sorular
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790352"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office Dağıtım Aracı'nı (ODT) kullanma hakkında sorular

Microsoft İndirme Merkezi'nden Office [Dağıtım Aracı'nı indirin.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir dosyasını (setup.exe) ve örnek bir yapılandırma dosyasını (yürütülebilir) içeren, otomatik olarak ayıklanan yürütülebilir dosyayı configuration.xml.
  
 **Kurumsal ürünler için Microsoft 365 Uygulamalarını istemci bilgisayarlardan çıkarmak veya hariç tutmak için:**
  
Microsoft 365 Uygulamalarını kuruluş için yüklerken belirli ürünleri hariç tutabilirsiniz. Bunu yapmak için, ODT ile Office'i yükleme adımlarını izleyin, ancak yapılandırma dosyanıza ExcludeApp öğesini de dahil edin. Örneğin, bu yapılandırma dosyası Publisher dışındaki kurumsal ürünler için tüm Microsoft 365 Uygulamalarını yüklemektedir:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office Dağıtım Aracı'nı genel bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

