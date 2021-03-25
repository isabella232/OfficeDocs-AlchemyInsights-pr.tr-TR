---
title: RDS, Terminal Server veya VDI'de paylaşılan kullanım için kuruluş için Microsoft 365 Uygulamalarını dağıtma
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200693"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS, Terminal Server veya VDI'de paylaşılan kullanım için kuruluş için Microsoft 365 Uygulamalarını dağıtma

Eski adı Terminal Hizmetleri olan Uzak Masaüstü Hizmetleri'ni (RDS) kullanarak kuruluşa Microsoft 365 Uygulamalarını dağıtmak için:

- Microsoft 365 İş planınız veya Office 365 Kurumsal E3 veya Kurumsal E5 gibi kurumsal Microsoft 365 Uygulamaları içeren bir Office 365 planınız olması gerekir.
   > [!NOTE]
   > İşletmeler için Microsoft 365 Uygulamaları ve Microsoft 365 İş Standart planları, kuruluş için Microsoft 365 Uygulamalarını içermez.
- Paylaşılan bilgisayar [etkinleştirmeyi etkinleştirmeniz gerekir.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Ayrıca, paylaşılan bilgisayar etkinleştirme modunda [kuruluş için Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) 365 Uygulamalarını yüklemek için Microsoft Destek ve Kurtarma Yardımcısı'ı indirip çalıştırabilirsiniz.

Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeler hakkında önkoşullar, kurulum yönergeleri ve yönergeler hakkında daha fazla bilgi için, Uzak Masaüstü Hizmetleri'nı kullanarak kuruluş için [Microsoft 365 Uygulamalarını Dağıtma'ya bakın.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:

- Kurumsal [Microsoft 365 Uygulamaları için paylaşılan bilgisayar etkinleştirme sorunlarını giderme makalesine bakın.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Bkz. [Kuruluşlar için Microsoft 365 Uygulamaları etkinleştirme durumunu sıfırlama](https://go.microsoft.com/fwlink/?linkid=2109218).

Varsayılan yükleme ayarlarını kullanan Microsoft 365 yönetim merkezinden RDS'ye kuruluş için Microsoft 365 Uygulamalarını yüklemek için ***aşağıdaki*** adımları kullanın:

1. Hangi aboneliğe sahip olduğunu kontrol edin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Gerekirse farklı bir aboneliğe geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Office diğer Microsoft aboneliklerini kullanarak RDS sunucusuna zaten yüklenmişse kaldırın. Örneğin Denetim Masası'nı **kullanarak**  >  **programı kaldırın.** Microsoft Destek [ve Kurtarma Yardımcısı'nın](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanımıyla ilgili sorunlar ile ilgili sorunları kaldırın.
4. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetim merkezinde oturum açın ve kuruluş için [Microsoft 365 Uygulamalarını yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)
5. Office yüklendikten sonra hiçbir Office ***uygulaması açmayın veya*** oturum açmayın.
6. RDS sunucusunda, aşağıdaki adımları kullanarak kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:
   1. Ekranın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı **seçin.** Aç kutusuna, **regedit** yazın ve sonra da **Tamam**'ı seçin.
   2. Kayıt **Defteri** Düzenleyicisi'nin aygıtınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.
   3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarıyla **SharedComputerLicensing'in** dize değerini ekleyin.
   4. RDS sunucusunda ***son*** kullanıcı olarak oturum açma ve kuruluş için Microsoft 365 Uygulamaları için paylaşılan bilgisayar etkinleştirmenin [etkinleştirildiğinden emin olun.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
