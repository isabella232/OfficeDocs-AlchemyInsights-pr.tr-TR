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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="74cbb-102">Office dağıtım aracı 'nı (ODT) kullanma hakkında sorular</span><span class="sxs-lookup"><span data-stu-id="74cbb-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="74cbb-103">Office dağıtım aracı 'nı [Microsoft Yükleme Merkezi](https://go.microsoft.com/fwlink/p/?LinkID=626065)'nden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="74cbb-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="74cbb-104">Dosyayı indirdikten sonra, Office dağıtım Aracı yürütülebilir (setup.exe) ve örnek yapılandırma dosyası (configuration.xml) içeren kendiliğinden ayıklanan yürütülebilir dosyayı çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="74cbb-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="74cbb-105">**Kurumsal Ürünler için Microsoft 365 uygulamalarını istemci bilgisayarlardan dışlamak veya kaldırmak için:**</span><span class="sxs-lookup"><span data-stu-id="74cbb-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="74cbb-106">Kuruluş için Microsoft 365 uygulamalarını yüklerken belirli ürünleri dışlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="74cbb-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="74cbb-107">Bunu yapmak için, Office 'i ODT ile yükleme adımlarını izleyin, ancak yapılandırma dosyanıza ExcludeApp öğesini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="74cbb-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="74cbb-108">Örneğin, bu yapılandırma dosyası Publisher dışında kurumsal ürünler için Microsoft 365 uygulamalarını yükler:</span><span class="sxs-lookup"><span data-stu-id="74cbb-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="74cbb-109">Office dağıtım aracına genel bakış</span><span class="sxs-lookup"><span data-stu-id="74cbb-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

