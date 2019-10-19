---
title: Office Dağıtım Aracının (ODT) nasıl kullanılacağı yla ilgili sorular
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553560"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="54d25-102">Office Dağıtım Aracının (ODT) nasıl kullanılacağı yla ilgili sorular</span><span class="sxs-lookup"><span data-stu-id="54d25-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="54d25-103">Office Dağıtım Aracını [Microsoft İndirme Merkezi'nden](http://go.microsoft.com/fwlink/p/?LinkID=626065)indirin.</span><span class="sxs-lookup"><span data-stu-id="54d25-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="54d25-104">Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir (setup.exe) ve örnek yapılandırma dosyasını (configuration.xml) içeren kendi kendini ayıklayan yürütülebilir dosyayı çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="54d25-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="54d25-105">**Office 365 ProPlus ürünlerini istemci bilgisayarlardan hariç tutmak veya kaldırmak için:**</span><span class="sxs-lookup"><span data-stu-id="54d25-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="54d25-106">Office 365 ProPlus'ı yüklerken, belirli ürünleri hariç tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="54d25-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="54d25-107">Bunu yapmak için Office'i ODT ile yükleme adımlarını izleyin, ancak yapılandırma dosyanıza DışUygulama öğesini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="54d25-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="54d25-108">Örneğin, bu yapılandırma dosyası Publisher dışındaki tüm Office 365 ProPlus ürünlerini yükler:</span><span class="sxs-lookup"><span data-stu-id="54d25-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="54d25-109">Office Dağıtım Aracına Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="54d25-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

