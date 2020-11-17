---
title: Office dağıtım aracı 'nı kullanma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085852"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="6ed4f-102">Office dağıtım aracı 'nı (ODT) kullanma</span><span class="sxs-lookup"><span data-stu-id="6ed4f-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6ed4f-103">Office dağıtım aracı 'nı (ODT) kullanarak Office 'in Office 365 sürümlerini dağıtabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="6ed4f-104">Office dağıtım aracı (setupodt.exe) komut satırından çalıştırılır ve Office dağıtılırken uygulanacak ayarları belirlemek için bir yapılandırma XML dosyası kullanır.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="6ed4f-105">Office dağıtım aracı 'nın en son sürümünü [Microsoft Yükleme Merkezi](https://go.microsoft.com/fwlink/p/?LinkID=626065)'nden indirin.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="6ed4f-106">[Office Özelleştirme Aracı 'nı (OCT)](https://config.office.com) kullanarak dağıtım tercihlerinizi seçin ve yapılandırma XML dosyasını oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="6ed4f-107">Yapılandırma dosyasını dışarı aktarın ve setupodt.exe bulunduğu klasöre yerel olarak yerleştirin.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="6ed4f-108">**Not:** Office yükleme sorunları genellikle yanlış yapılandırılmış veya malbiçimli yapılandırma dosyaları nedeniyle gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="6ed4f-109">Bu sorunlardan kaçınmak için, yapılandırma dosyasını oluşturmak için Office Özelleştirme Aracı 'nı kullanmanızı öneririz.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="6ed4f-110">Ayrıca, varolan yapılandırma dosyalarını Office özelleştirme aracına da aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="6ed4f-111">Yükseltilmiş bir komut isteminden, setupodt.exe bulunduğu konuma geçin ve Office dağıtım aracı 'nı indirme modunda çalıştırır ve az önce kaydettiğiniz yapılandırma dosyasını belirtin.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="6ed4f-112">Bu örnekte, yapılandırma dosyası Configuration.xml olarak adlandırılır:</span><span class="sxs-lookup"><span data-stu-id="6ed4f-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="6ed4f-113">4. Office dağıtım aracı 'nı Yapılandır modunda çalıştırıp yapılandırma dosyasını belirtin.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="6ed4f-114">**Not:** Bu adımı, Office 'i yüklemek istediğiniz istemci bilgisayarda çalıştırmalısınız ve bu bilgisayarda yerel yönetici izinleriniz olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="6ed4f-115">Microsoft 365 uygulamalarınız için Office dağıtım aracı 'nı kurumsal dağıtım senaryolarında kullanma konusunda daha fazla bilgi edinmek için, [Office dağıtım aracı 'Na genel bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="6ed4f-116">Office Özelleştirme Aracı 'nı kullanma hakkında daha fazla bilgi için, [Office özelleştirme aracına genel bakış](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="6ed4f-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
