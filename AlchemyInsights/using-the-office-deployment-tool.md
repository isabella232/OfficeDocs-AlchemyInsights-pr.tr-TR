---
title: Office Dağıtım Aracı'nı kullanma
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531595"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office Dağıtım Aracı'nın (ODT)

Office Dağıtım Aracı'nın (ODT), Office 365 Office sürümlerini dağıtmak için kullanın. Office Dağıtım Aracı'nı (setup.exe) komut satırından çalıştırın ve Office dağıtırken uygulanacak ayarları belirlemek üzere bir yapılandırma XML dosyası kullanır.
  
1. En son sürümü Office dağıtım aracı [Microsoft Yükleme Merkezi'nden](http://go.microsoft.com/fwlink/p/?LinkID=626065)yükleyin.

2. Dağıtım tercihlerinizi seçin ve XML yapılandırma dosyası oluşturmak için [Office Özelleştirme Aracı'nı (OCT)](https://config.office.com) kullanın. Yapılandırma dosyasını verme ve aynı klasörde setup.exe bulunduğu yerel olarak yerleştirin.

    **Not:** Malformatted yapılandırma dosyaları veya office yükleme sorunları genellikle son için yapılandırılmış oluşur. Bu tür sorunları önlemek için yapılandırma dosyası oluşturmak için Office Özelleştirme Aracı'nı kullanmanızı öneririz. Ayrıca, Office Özelleştirme Aracı'nı varolan yapılandırma dosyalarını içe aktarabilirsiniz.

3. Yükseltilmiş bir komut isteminden setup.exe bulunduğu konuma geçin ve Office Dağıtım Aracı'nı karşıdan yükleme modunda çalıştırın ve az önce kaydettiğiniz yapılandırma dosyası belirtin. Bu örnekte, yapılandırma dosyası Configuration.xml olarak adlandırılır:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Office Dağıtım Aracı'nı çalıştırma modunda yapılandırın ve yapılandırma dosyası belirtin.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Not:** Bu adımı, Office'i yüklemek istediğiniz ve o bilgisayarda yerel yönetici izinlerine sahip istemci bilgisayardan çalıştırmalısınız.

Office 365 ProPlus, dağıtım senaryolarınız için Office dağıtım aracı kullanma hakkında daha fazla bilgi için bkz: [Office dağıtım aracı genel bakış](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Office Özelleştirme Aracı'nı kullanma hakkında daha fazla bilgi için bkz: [Office Özelleştirme Aracı'nı genel bakış](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
