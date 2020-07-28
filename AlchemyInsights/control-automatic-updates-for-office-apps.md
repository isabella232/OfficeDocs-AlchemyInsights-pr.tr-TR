---
title: Office Uygulamaları için otomatik güncelleştirmeleri denetleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439928"
---
# <a name="control-automatic-updates-for-office-apps"></a>Office Uygulamaları için otomatik güncelleştirmeleri denetleme

Varsayılan olarak, Office Apps güncelleştirmeleri otomatik olarak indirilir ve herhangi bir kullanıcı müdahalesi olmadan arka planda uygulanır. Ancak yöneticiler, Office Update ayarlarını kullanarak güncelleştirmelerin nasıl uygulandığını denetleyebilir. Güncelleştirme ayarları, yöneticilerin otomatik güncelleştirmeleri etkinleştirmesine veya devre dışı bırakarak Office'te **Şimdi Güncelleştir** düğmesini göstermesine veya gizlemesine, güncelleştirme son tarihlerini ayarlamasına ve daha fazlasını sağlamasına olanak tanır. Ayrıntılı bilgi için bkz:

- [Office için güncelleştirme ayarlarını yapılandırma](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office için otomatik güncelleştirme etkinleştirildi](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Office yüklendikten sonra nasıl güncelleştirin](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

İstemci makinesine uygulanan varolan güncelleştirme ayarlarını gözden geçirmek için aşağıdaki adımları izleyin:

1. **Başlat**  >  **Çalıştır**  >  **regedit'e**giderek Kayıt Defteri Düzenleyicisini açın.
2. Aşağıdaki konuma geçin ve Office Güncelleştirmesi ayarlarını gözden geçirin:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Yapılandırma

**Not**  OfficeMgmtCOM anahtarı ayarlanmışsa, **Office**  >  **Hesap**  >  **Ofisi Güncelleştirmeleri'nde**"Güncelleştirmeler sistem yöneticiniz tarafından yönetilir" iletisini görebilirsiniz. Daha fazla bilgi için Microsoft [Endpoint Configuration Manager ile Microsoft 365 Uygulamalarındaki güncelleştirmeleri yönet'e](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)bakın.  