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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="75ab3-102">Office Dağıtım Aracı'nı (ODT) kullanma hakkında sorular</span><span class="sxs-lookup"><span data-stu-id="75ab3-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="75ab3-103">Microsoft İndirme Merkezi'nden Office [Dağıtım Aracı'nı indirin.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="75ab3-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="75ab3-104">Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir dosyasını (setup.exe) ve örnek bir yapılandırma dosyasını (yürütülebilir) içeren, otomatik olarak ayıklanan yürütülebilir dosyayı configuration.xml.</span><span class="sxs-lookup"><span data-stu-id="75ab3-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="75ab3-105">**Kurumsal ürünler için Microsoft 365 Uygulamalarını istemci bilgisayarlardan çıkarmak veya hariç tutmak için:**</span><span class="sxs-lookup"><span data-stu-id="75ab3-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="75ab3-106">Microsoft 365 Uygulamalarını kuruluş için yüklerken belirli ürünleri hariç tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="75ab3-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="75ab3-107">Bunu yapmak için, ODT ile Office'i yükleme adımlarını izleyin, ancak yapılandırma dosyanıza ExcludeApp öğesini de dahil edin.</span><span class="sxs-lookup"><span data-stu-id="75ab3-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="75ab3-108">Örneğin, bu yapılandırma dosyası Publisher dışındaki kurumsal ürünler için tüm Microsoft 365 Uygulamalarını yüklemektedir:</span><span class="sxs-lookup"><span data-stu-id="75ab3-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="75ab3-109">Office Dağıtım Aracı'nı genel bakış</span><span class="sxs-lookup"><span data-stu-id="75ab3-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

