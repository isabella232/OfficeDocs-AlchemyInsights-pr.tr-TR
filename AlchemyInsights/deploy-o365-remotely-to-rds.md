---
title: RDS Kurumlar için Microsoft 365 Uygulamaları Terminal Sunucusu veya VDI'de paylaşılan kullanım için dağıtım
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031498"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS Kurumlar için Microsoft 365 Uygulamaları Terminal Sunucusu veya VDI'de paylaşılan kullanım için dağıtım

Uzak Masaüstü Kurumlar için Microsoft 365 Uygulamaları (RDS) kullanarak terminal dağıtımı yapmak için(eski adı Terminal Hizmetleri):

- E3 veya Microsoft 365 E5 gibi Kurumlar için Microsoft 365 Uygulamaları içeren bir Office 365 İş planınız Office 365 Kurumsal Enterprise gerekir.
   > [!NOTE]
   > Planlar İş için Microsoft 365 Uygulamaları Microsoft 365 İş Standart planlarında yeni özellikler Kurumlar için Microsoft 365 Uygulamaları.
- Paylaşılan bilgisayar [etkinleştirmeyi etkinleştirmeniz gerekir.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Ayrıca, paylaşılan bilgisayar etkinleştirme modunda Destek ve Kurtarma Yardımcısı [için Microsoft Kurumlar için Microsoft 365 Uygulamaları'ni](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.

Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeler hakkında önkoşullar, kurulum yönergeleri ve yönergeler hakkında daha fazla bilgi için bkz. Uzak Masaüstü Hizmetleri kullanarak [Kurumlar için Microsoft 365 Uygulamaları'i dağıtma.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Paylaşılan bilgisayar etkinleştirmesi ile ilgili hataları düzeltmek için:

- Daha [fazla bilgi için bkz. Paylaşılan bilgisayar etkinleştirme Kurumlar için Microsoft 365 Uygulamaları.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Bkz. [Kuruluşlar için Microsoft 365 Uygulamaları etkinleştirme durumunu sıfırlama](https://go.microsoft.com/fwlink/?linkid=2109218).

varsayılan yükleme ayarlarını kullanan Kurumlar için Microsoft 365 Uygulamaları RDS'Microsoft 365 yönetim merkezi rds üzerine yüklemek için aşağıdaki adımları kullanın:

1. Hangi aboneliğe sahip olduğunu kontrol edin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Gerekirse farklı bir aboneliğe geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Diğer Office Microsoft aboneliklerini kullanarak RDS sunucusuna zaten yüklenmişse kaldırın. Örneğin Denetim Masası'nı **kullanarak**  >  **Program kaldır'ı seçin.** Sorun [Destek ve Kurtarma Yardımcısı](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft Destek ve Kurtarma Yardımcısı'ı kullanarak programı kaldırın.
4. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetim merkezi oturum açın ve yükleme [Kurumlar için Microsoft 365 Uygulamaları.](https://portal.office.com/OLS/MySoftware.aspx)
5. Yükleme Office, herhangi bir ***uygulama açmayın veya Office*** açın.
6. RDS sunucusunda, aşağıdaki adımları takip edin ve kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:
   1. Ekranın sol alt Windows Seçenekler düğmesine sağ tıklayın ve Çalıştır'ı **seçin.** Aç kutusuna, **regedit** yazın ve sonra da **Tamam**'ı seçin.
   2. Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmaya izin vermesine izin vermek istendiğinde Evet'i seçin.
   3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarıyla **SharedCompcomplicensing** dize değeri ekleyin.
   4. RDS sunucusunda, son ***kullanıcı olarak oturum açma ve*** son kullanıcı için paylaşılan bilgisayar [etkinleştirmenin etkinleştirildiğinden emin Kurumlar için Microsoft 365 Uygulamaları.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
