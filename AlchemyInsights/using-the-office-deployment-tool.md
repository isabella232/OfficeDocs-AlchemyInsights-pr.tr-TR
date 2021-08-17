---
title: Office Dağıtım Aracı'nı kullanma
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083790"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office Dağıtım Aracı'nı (ODT) kullanma

Office Dağıtım Aracı'nı (ODT) kullanarak, Office 365 sürümlerinin dağıtımını Office. En Office Dağıtım Aracı (setup.exe) komut satırından çalıştırlanır ve bu aracı dağıtırken hangi ayarların uygulanacaklarını belirlemek için bir yapılandırma XML Office.
  
1. Microsoft İndirme Merkezi'nden Office Dağıtım Aracı'nın [en son sürümünü indirin.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Dağıtım [tercihlerinizi Office ve yapılandırma](https://config.office.com) XML dosyasını oluşturmak için Gelişmiş Özelleştirme Aracı'nı (OCT) kullanın. Yapılandırma dosyasını dışarı aktarın ve yerel olarak dosyanın bulunduğu klasöre setup.exe.

    **Not:** Office yanlış yapılandırılmış veya yanlış biçimlendirilmiş yapılandırma dosyaları nedeniyle genellikle yükleme sorunları oluşur. Bu tür sorunları önlemek için, yapılandırma dosyasını Office Özelleştirme Aracı'nı kullanmanızı öneririz. Ayrıca, var olan yapılandırma dosyalarını Özelleştirme Aracı'Office aktarabilirsiniz.

3. Yükseltilmiş komut isteminden, setup.exe bulunduğu konuma geçiş Office karşıdan yükleme modunda Office yapılandırma dosyasını belirtin. Bu örnekte, yapılandırma dosyasının adı şu Configuration.xml:

```setup.exe /download Configuration.xml```

4.Yapılandırma Office için Dağıtım Aracı'nı çalıştırın ve yapılandırma dosyasını belirtin.

```setup.exe /configure Configuration.xml```

**Not:** Bu adımı, e-posta yüklemesini istediğiniz istemci bilgisayarda Office ve bu bilgisayarda yerel yönetici izinlerine sahip olmak gerekir.

Microsoft Dağıtım Aracı'nı Office senaryolarında kullanma hakkında daha Kurumlar için Microsoft 365 Uygulamaları için bkz. Dağıtım Aracı'Office [genel bakış.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Özelleştirme Aracı'nın kullanımı hakkında daha fazla Office için bkz. Özelleştirme [Aracı'Office genel bakış.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
