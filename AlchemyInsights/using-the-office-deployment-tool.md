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
# <a name="using-the-office-deployment-tool-odt"></a>Office dağıtım aracı 'nı (ODT) kullanma

Office dağıtım aracı 'nı (ODT) kullanarak Office 'in Office 365 sürümlerini dağıtabilirsiniz. Office dağıtım aracı (setupodt.exe) komut satırından çalıştırılır ve Office dağıtılırken uygulanacak ayarları belirlemek için bir yapılandırma XML dosyası kullanır.
  
1. Office dağıtım aracı 'nın en son sürümünü [Microsoft Yükleme Merkezi](https://go.microsoft.com/fwlink/p/?LinkID=626065)'nden indirin.

2. [Office Özelleştirme Aracı 'nı (OCT)](https://config.office.com) kullanarak dağıtım tercihlerinizi seçin ve yapılandırma XML dosyasını oluşturun. Yapılandırma dosyasını dışarı aktarın ve setupodt.exe bulunduğu klasöre yerel olarak yerleştirin.

    **Not:** Office yükleme sorunları genellikle yanlış yapılandırılmış veya malbiçimli yapılandırma dosyaları nedeniyle gerçekleşir. Bu sorunlardan kaçınmak için, yapılandırma dosyasını oluşturmak için Office Özelleştirme Aracı 'nı kullanmanızı öneririz. Ayrıca, varolan yapılandırma dosyalarını Office özelleştirme aracına da aktarabilirsiniz.

3. Yükseltilmiş bir komut isteminden, setupodt.exe bulunduğu konuma geçin ve Office dağıtım aracı 'nı indirme modunda çalıştırır ve az önce kaydettiğiniz yapılandırma dosyasını belirtin. Bu örnekte, yapılandırma dosyası Configuration.xml olarak adlandırılır:

```setupodt.exe /download Configuration.xml```

4. Office dağıtım aracı 'nı Yapılandır modunda çalıştırıp yapılandırma dosyasını belirtin.

```setupodt.exe /configure Configuration.xml```

**Not:** Bu adımı, Office 'i yüklemek istediğiniz istemci bilgisayarda çalıştırmalısınız ve bu bilgisayarda yerel yönetici izinleriniz olmalıdır.

Microsoft 365 uygulamalarınız için Office dağıtım aracı 'nı kurumsal dağıtım senaryolarında kullanma konusunda daha fazla bilgi edinmek için, [Office dağıtım aracı 'Na genel bakış](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)konusuna bakın. Office Özelleştirme Aracı 'nı kullanma hakkında daha fazla bilgi için, [Office özelleştirme aracına genel bakış](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)konusuna bakın.
