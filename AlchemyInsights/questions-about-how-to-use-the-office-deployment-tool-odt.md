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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959703"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office Dağıtım Aracı'nı (ODT) kullanma hakkında sorular

Microsoft İndirme Office'nden İndirme Dağıtım [Aracı'nı indirin.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir dosyasını (setup.exe) ve örnek bir yapılandırma dosyasını (yürütülebilir) içeren, kendi kendine ayıklanan yürütülebilir dosyayı configuration.xml.
  
 **İstemci bilgisayarlarında, Kurumlar için Microsoft 365 Uygulamaları dışında tutmak veya kaldırmak için:**
  
E-Kurumlar için Microsoft 365 Uygulamaları belirli ürünleri hariç tutabilirsiniz. Bunu yapmak için, ODT'Office yükleme adımlarını izleyin, ancak yapılandırma dosyanıza ExcludeApp öğesini de dahil edin. Örneğin, bu yapılandırma dosyası aşağıdakiler dışında Kurumlar için Microsoft 365 Uygulamaları tüm Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office Dağıtım Aracı'nı Genel Bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

