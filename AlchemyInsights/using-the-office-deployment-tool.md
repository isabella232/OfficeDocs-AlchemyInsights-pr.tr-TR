---
title: Office Dağıtım Aracını Kullanma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726268"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="8f313-102">Office Dağıtım Aracını Kullanma (ODT)</span><span class="sxs-lookup"><span data-stu-id="8f313-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="8f313-103">Office'in Office 365 sürümlerini dağıtmak için Office Dağıtım Aracı'nı (ODT) kullanırsınız.</span><span class="sxs-lookup"><span data-stu-id="8f313-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="8f313-104">Office Dağıtım Aracı (setup.exe) komut satırından çalıştırılır ve Office'i dağıtırken hangi ayarların uygulanacağınızı belirlemek için bir yapılandırma XML dosyası kullanır.</span><span class="sxs-lookup"><span data-stu-id="8f313-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="8f313-105">[Microsoft Download Center'dan](https://go.microsoft.com/fwlink/p/?LinkID=626065)Office Dağıtım Aracı'nın en son sürümünü indirin.</span><span class="sxs-lookup"><span data-stu-id="8f313-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="8f313-106">Dağıtım tercihlerinizi seçmek ve yapılandırma XML dosyasını oluşturmak için [Office Özelleştirme Aracı'nı (OCT)](https://config.office.com) kullanın.</span><span class="sxs-lookup"><span data-stu-id="8f313-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="8f313-107">Yapılandırma dosyasını dışa aktarın ve setup.exe'nin bulunduğu klasöre yerel olarak yerleştirin.</span><span class="sxs-lookup"><span data-stu-id="8f313-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="8f313-108">**Not:** Office yükleme sorunları genellikle yanlış yapılandırılmış veya biçimlendirilmiş yapılandırma dosyaları nedeniyle oluşur.</span><span class="sxs-lookup"><span data-stu-id="8f313-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="8f313-109">Bu tür sorunları önlemek için, yapılandırma dosyasını oluşturmak için Office Özelleştirme Aracı'nı kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="8f313-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="8f313-110">Varolan yapılandırma dosyalarını Office Özelleştirme Aracına da aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8f313-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="8f313-111">Yükseltilmiş bir komut isteminden, setup.exe'nin bulunduğu konuma geçin ve Office Dağıtım Aracı'nı indirme modunda çalıştırın ve az önce kaydettiğiniz yapılandırma dosyasını belirtin.</span><span class="sxs-lookup"><span data-stu-id="8f313-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="8f313-112">Bu örnekte, yapılandırma dosyası Configuration.xml adlı:</span><span class="sxs-lookup"><span data-stu-id="8f313-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="8f313-113">Office Dağıtım Aracını yapılandırma modunda çalıştırın ve yapılandırma dosyasını belirtin.</span><span class="sxs-lookup"><span data-stu-id="8f313-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="8f313-114">**Not:** Bu adımı Office'i yüklemek istediğiniz istemci bilgisayardan çalıştırmanız ve bu bilgisayarda yerel yönetici izinlerine sahip olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="8f313-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="8f313-115">Kurumsal dağıtım senaryoları için Microsoft 365 Uygulamalarınız için Office Dağıtım [Aracı'nı](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)kullanma hakkında daha fazla bilgi edinmek için Bkz.</span><span class="sxs-lookup"><span data-stu-id="8f313-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="8f313-116">Office Özelleştirme Aracı'nın nasıl kullanılacağı hakkında daha fazla bilgi için Bkz. [Office Özelleştirme Aracı'na Genel Bakış.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)</span><span class="sxs-lookup"><span data-stu-id="8f313-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
