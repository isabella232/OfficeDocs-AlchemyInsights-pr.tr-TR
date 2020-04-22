---
title: Office Dağıtım Aracının (ODT) nasıl kullanılacağı yla ilgili sorular
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698078"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office Dağıtım Aracının (ODT) nasıl kullanılacağı yla ilgili sorular

Office Dağıtım Aracını [Microsoft İndirme Merkezi'nden](https://go.microsoft.com/fwlink/p/?LinkID=626065)indirin.
  
Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir (setup.exe) ve örnek yapılandırma dosyasını (configuration.xml) içeren kendi kendini ayıklayan yürütülebilir dosyayı çalıştırın.
  
 **Kurumsal ürünler için Microsoft 365 Uygulamalarını istemci bilgisayarlardan hariç tutmak veya kaldırmak için:**
  
Kurumsal microsoft 365 Apps yüklerken, belirli ürünleri hariç tutabilirsiniz. Bunu yapmak için Office'i ODT ile yükleme adımlarını izleyin, ancak yapılandırma dosyanıza DışUygulama öğesini ekleyin. Örneğin, bu yapılandırma dosyası Publisher dışındaki kurumsal ürünler için tüm Microsoft 365 Uygulamalarını yükler:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office Dağıtım Aracına Genel Bakış](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

