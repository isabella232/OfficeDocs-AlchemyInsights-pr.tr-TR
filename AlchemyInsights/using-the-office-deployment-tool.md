---
title: Office Dağıtım Aracı'nı kullanma
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898670"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="cc076-102">Office Dağıtım Aracı'nın (ODT)</span><span class="sxs-lookup"><span data-stu-id="cc076-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="cc076-p101">Office Dağıtım Aracı'nın (ODT), Office 365 Office sürümlerini dağıtmak için kullanın. Office Dağıtım Aracı'nı (setup.exe) komut satırından çalıştırın ve Office dağıtırken uygulanacak ayarları belirlemek üzere bir yapılandırma XML dosyası kullanır.</span><span class="sxs-lookup"><span data-stu-id="cc076-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="cc076-105">En son sürümü Office dağıtım aracı [Microsoft Yükleme Merkezi'nden](http://go.microsoft.com/fwlink/p/?LinkID=626065)yükleyin.</span><span class="sxs-lookup"><span data-stu-id="cc076-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="cc076-p102">Dağıtım tercihlerinizi seçin ve XML yapılandırma dosyası oluşturmak için [Office Özelleştirme Aracı'nı (OCT)](https://config.office.com) kullanın. Yapılandırma dosyasını verme ve aynı klasörde setup.exe bulunduğu yerel olarak yerleştirin.</span><span class="sxs-lookup"><span data-stu-id="cc076-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="cc076-p103">**Not:** Malformatted yapılandırma dosyaları veya office yükleme sorunları genellikle son için yapılandırılmış oluşur. Bu tür sorunları önlemek için yapılandırma dosyası oluşturmak için Office Özelleştirme Aracı'nı kullanmanızı öneririz. Ayrıca, Office Özelleştirme Aracı'nı varolan yapılandırma dosyalarını içe aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="cc076-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="cc076-p104">Yükseltilmiş bir komut isteminden setup.exe bulunduğu konuma geçin ve Office Dağıtım Aracı'nı karşıdan yükleme modunda çalıştırın ve az önce kaydettiğiniz yapılandırma dosyası belirtin. Bu örnekte, yapılandırma dosyası Configuration.xml olarak adlandırılır:</span><span class="sxs-lookup"><span data-stu-id="cc076-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="cc076-113">Office Dağıtım Aracı'nı çalıştırma modunda yapılandırın ve yapılandırma dosyası belirtin.</span><span class="sxs-lookup"><span data-stu-id="cc076-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="cc076-114">**Not:** Bu adımı, Office'i yüklemek istediğiniz ve o bilgisayarda yerel yönetici izinlerine sahip istemci bilgisayardan çalıştırmalısınız.</span><span class="sxs-lookup"><span data-stu-id="cc076-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="cc076-p105">Office 365 ProPlus, dağıtım senaryolarınız için Office dağıtım aracı kullanma hakkında daha fazla bilgi için bkz: [Office dağıtım aracı genel bakış](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Office Özelleştirme Aracı'nı kullanma hakkında daha fazla bilgi için bkz: [Office Özelleştirme Aracı'nı genel bakış](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="cc076-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

