---
title: Office Dağıtım Aracı'nın (ODT) kullanma hakkında sorular
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494837"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="40715-102">Office Dağıtım Aracı'nın (ODT) kullanma hakkında sorular</span><span class="sxs-lookup"><span data-stu-id="40715-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="40715-103">Office dağıtım aracı [Microsoft Yükleme Merkezi'nden](http://go.microsoft.com/fwlink/p/?LinkID=626065)yükleyin.</span><span class="sxs-lookup"><span data-stu-id="40715-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="40715-104">Dosyayı karşıdan yükledikten sonra Office dağıtım aracı yürütülebilir (setup.exe) içeren kendi kendine ayıklanan yürütülebilir dosya ve örnek bir yapılandırma dosyası (configuration.xml) çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="40715-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="40715-105">**Dışarıda veya Office 365 ProPlus ürün istemci bilgisayarlardan kaldırmak için:**</span><span class="sxs-lookup"><span data-stu-id="40715-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="40715-p101">Office 365 ProPlus yüklerken, belirli ürünleri dışlayabilirsiniz. Bunu yapmak için ODT ile Office yüklemek için adımları izleyin, ancak ExcludeApp öğesi yapılandırma dosyanıza ekleyin. Örneğin, Publisher dışındaki tüm Office 365 ProPlus ürünleri bu yapılandırma dosyası yükler:</span><span class="sxs-lookup"><span data-stu-id="40715-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="40715-109">Office dağıtım aracı genel bakış</span><span class="sxs-lookup"><span data-stu-id="40715-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

