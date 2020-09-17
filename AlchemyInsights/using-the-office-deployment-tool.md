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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794931"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office dağıtım aracı 'nı (ODT) kullanma

Office dağıtım aracı 'nı (ODT) kullanarak Office 'in Office 365 sürümlerini dağıtabilirsiniz. Office dağıtım aracı (setup.exe) komut satırından çalıştırılır ve Office dağıtılırken uygulanacak ayarları belirlemek için bir yapılandırma XML dosyası kullanır.
  
1. Office dağıtım aracı 'nın en son sürümünü [Microsoft Yükleme Merkezi](https://go.microsoft.com/fwlink/p/?LinkID=626065)'nden indirin.

2. [Office Özelleştirme Aracı 'nı (OCT)](https://config.office.com) kullanarak dağıtım tercihlerinizi seçin ve yapılandırma XML dosyasını oluşturun. Yapılandırma dosyasını dışarı aktarın ve setup.exe bulunduğu klasöre yerel olarak yerleştirin.

    **Not:** Office yükleme sorunları genellikle yanlış yapılandırılmış veya malbiçimli yapılandırma dosyaları nedeniyle gerçekleşir. Bu sorunlardan kaçınmak için, yapılandırma dosyasını oluşturmak için Office Özelleştirme Aracı 'nı kullanmanızı öneririz. Ayrıca, varolan yapılandırma dosyalarını Office özelleştirme aracına da aktarabilirsiniz.

3. Yükseltilmiş bir komut isteminden, setup.exe bulunduğu konuma geçin ve Office dağıtım aracı 'nı indirme modunda çalıştırır ve az önce kaydettiğiniz yapılandırma dosyasını belirtin. Bu örnekte, yapılandırma dosyası Configuration.xml olarak adlandırılır:

```setup.exe /download Configuration.xml```

4. Office dağıtım aracı 'nı Yapılandır modunda çalıştırıp yapılandırma dosyasını belirtin.

```setup.exe /configure Configuration.xml```

**Not:** Bu adımı, Office 'i yüklemek istediğiniz istemci bilgisayarda çalıştırmalısınız ve bu bilgisayarda yerel yönetici izinleriniz olmalıdır.

Microsoft 365 uygulamalarınız için Office dağıtım aracı 'nı kurumsal dağıtım senaryolarında kullanma konusunda daha fazla bilgi edinmek için, [Office dağıtım aracı 'Na genel bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)konusuna bakın. Office Özelleştirme Aracı 'nı kullanma hakkında daha fazla bilgi için, [Office özelleştirme aracına genel bakış](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)konusuna bakın.
