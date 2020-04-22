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
# <a name="using-the-office-deployment-tool-odt"></a>Office Dağıtım Aracını Kullanma (ODT)

Office'in Office 365 sürümlerini dağıtmak için Office Dağıtım Aracı'nı (ODT) kullanırsınız. Office Dağıtım Aracı (setup.exe) komut satırından çalıştırılır ve Office'i dağıtırken hangi ayarların uygulanacağınızı belirlemek için bir yapılandırma XML dosyası kullanır.
  
1. [Microsoft Download Center'dan](https://go.microsoft.com/fwlink/p/?LinkID=626065)Office Dağıtım Aracı'nın en son sürümünü indirin.

2. Dağıtım tercihlerinizi seçmek ve yapılandırma XML dosyasını oluşturmak için [Office Özelleştirme Aracı'nı (OCT)](https://config.office.com) kullanın. Yapılandırma dosyasını dışa aktarın ve setup.exe'nin bulunduğu klasöre yerel olarak yerleştirin.

    **Not:** Office yükleme sorunları genellikle yanlış yapılandırılmış veya biçimlendirilmiş yapılandırma dosyaları nedeniyle oluşur. Bu tür sorunları önlemek için, yapılandırma dosyasını oluşturmak için Office Özelleştirme Aracı'nı kullanmanızı öneririz. Varolan yapılandırma dosyalarını Office Özelleştirme Aracına da aktarabilirsiniz.

3. Yükseltilmiş bir komut isteminden, setup.exe'nin bulunduğu konuma geçin ve Office Dağıtım Aracı'nı indirme modunda çalıştırın ve az önce kaydettiğiniz yapılandırma dosyasını belirtin. Bu örnekte, yapılandırma dosyası Configuration.xml adlı:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Office Dağıtım Aracını yapılandırma modunda çalıştırın ve yapılandırma dosyasını belirtin.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Not:** Bu adımı Office'i yüklemek istediğiniz istemci bilgisayardan çalıştırmanız ve bu bilgisayarda yerel yönetici izinlerine sahip olmalısınız.

Kurumsal dağıtım senaryoları için Microsoft 365 Uygulamalarınız için Office Dağıtım [Aracı'nı](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)kullanma hakkında daha fazla bilgi edinmek için Bkz. Office Özelleştirme Aracı'nın nasıl kullanılacağı hakkında daha fazla bilgi için Bkz. [Office Özelleştirme Aracı'na Genel Bakış.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
