---
title: Office uygulamaları için güncelleştirme kanallarını değiştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440024"
---
# <a name="change-update-channels-for-office-apps"></a>Office uygulamaları için güncelleştirme kanallarını değiştirme

Yeni Office yüklemeleri için, istenen güncelleştirme kanalını seçmek için Office Yazılım İndirme Ayarlarını kullanın ve ardından Office uygulamalarını yükleyin (veya yeniden yükleyin). Daha fazla bilgi için [Bkz. Office 365'teki yazılım indirme ayarlarını yönet.](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) 

**Not** Office Yazılım İndirme Ayarları kullanılarak seçilen güncelleştirme kanalı, O365 portalını kullanan yeni yüklemeler gerçekleştiren tüm kullanıcılar için geçerlidir. Daha fazla bilgi için microsoft [365 veya Office 2019'u bir PC veya Mac'te İndirve yükleyin veya yeniden yükleyin.](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)   

Varolan Office yüklemeleri için, farklı bir güncelleştirme kanalına geçmek için Office Dağıtım Aracı'nı (ODT) kullanın:  

1. [Microsoft Download Center'dan](https://go.microsoft.com/fwlink/p/?LinkID=626065)Office Dağıtım Aracı'nın (setup.exe) en son sürümünü indirin.
2. Geçmek istediğiniz kanalın adını tanımlayın. Daha fazla bilgi için [Office Dağıtım Aracı yapılandırma seçeneklerine](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)bakın.
3. Uygun kanal adını belirten bir yapılandırma XML dosyası oluşturun, örneğin, update.xml.  
    a. <Configuration>  
    b. <Güncellemeler **Kanalı="Aylık"** />  
    c. </Configuration>
4. Yükseltilmiş bir komut isteminden, setup.exe bulunduğu klasör konumuna geçin ve aşağıdaki komutu çalıştırın:  
    a. setup.exe /yapılandırma update.xml
5. Bir Office uygulamasını başlatın (Excel gibi) ve ardından **Dosya**  >  **Hesabı'nı**seçin. Ürün Bilgileri bölümünde, **Seçenekleri Şimdi**  >  **Güncelleştir'i**seçin.

Daha fazla bilgi için, [varolan Office Uygulamaları için güncelleştirme kanallarını nasıl değiştirin.](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

Seçili bir kullanıcı grubu için güncelleştirme kanallarını değiştirmek veya Configuration Manager (SCCM) kullanarak, GPO kullanarak Kanal Güncelleştirme ayarını yapılandırın. Daha fazla bilgi için Microsoft [365 Uygulamaları için güncelleştirme kanallarına genel bakış bölümüne](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)bakın. Ayrıntılar için BT [Uzmanları için Office 365 ProPlus Kanallarını nasıl yönetebilirsiniz](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) ve [Microsoft Endpoint Configuration Manager ile Microsoft 365 Uygulamalarındaki güncelleştirmeleri yönetme](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)konusuna bakın.