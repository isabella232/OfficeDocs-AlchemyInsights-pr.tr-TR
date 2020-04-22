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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="050db-102">Office Dağıtım Aracının (ODT) nasıl kullanılacağı yla ilgili sorular</span><span class="sxs-lookup"><span data-stu-id="050db-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="050db-103">Office Dağıtım Aracını [Microsoft İndirme Merkezi'nden](https://go.microsoft.com/fwlink/p/?LinkID=626065)indirin.</span><span class="sxs-lookup"><span data-stu-id="050db-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="050db-104">Dosyayı indirdikten sonra, Office Dağıtım Aracı yürütülebilir (setup.exe) ve örnek yapılandırma dosyasını (configuration.xml) içeren kendi kendini ayıklayan yürütülebilir dosyayı çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="050db-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="050db-105">**Kurumsal ürünler için Microsoft 365 Uygulamalarını istemci bilgisayarlardan hariç tutmak veya kaldırmak için:**</span><span class="sxs-lookup"><span data-stu-id="050db-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="050db-106">Kurumsal microsoft 365 Apps yüklerken, belirli ürünleri hariç tutabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="050db-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="050db-107">Bunu yapmak için Office'i ODT ile yükleme adımlarını izleyin, ancak yapılandırma dosyanıza DışUygulama öğesini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="050db-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="050db-108">Örneğin, bu yapılandırma dosyası Publisher dışındaki kurumsal ürünler için tüm Microsoft 365 Uygulamalarını yükler:</span><span class="sxs-lookup"><span data-stu-id="050db-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="050db-109">Office Dağıtım Aracına Genel Bakış</span><span class="sxs-lookup"><span data-stu-id="050db-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

