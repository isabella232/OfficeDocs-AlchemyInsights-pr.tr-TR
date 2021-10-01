---
title: RDS Microsoft 365 Uygulamaları Terminal Sunucusu veya VDI'de paylaşılan kullanım için dağıtım
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077270"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS Microsoft 365 Uygulamaları Terminal Sunucusu veya VDI'de paylaşılan kullanım için dağıtım

Uzak Masaüstü Microsoft 365 Uygulamaları (RDS) kullanarak terminal dağıtımı yapmak için, (eski adı Terminal Hizmetleri) şunları gerekir:

- Windows'un daha eski bir sürümünü (örneğin, Windows 7 SP1, Windows Server 2008 R2) kullanıyorsanız, kolay düzeltmeyi TLS 1.2'yi varsayılan olarak etkinleştirin. Kolay düzeltme ve daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi etkinleştirmek için Windows.](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy) 
- Kurumlar için Microsoft 365 Uygulamaları Plus'Office 365 planınız var. Örneğin, Office 365 E3 veya Microsoft 365 E5 ya da Project ya da Visio'un masaüstü sürümünü içeren herhangi bir planı (Project Plan 3 veya Visio Plan 2 gibi) ya da Microsoft 365 İş Ekstra planı da İş için Microsoft 365 Uygulamaları.
- Paylaşılan bilgisayar etkinleştirmeyi etkinleştirin. Daha fazla bilgi için [bkz. Microsoft için paylaşılan bilgisayar etkinleştirme Microsoft 365 Uygulamaları.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Not:** Paylaşılan Microsoft 365 Uygulamaları etkinleştirme modunda yükleme yapmak için Microsoft Etkinleştirme [Sihirbazı'Destek ve Kurtarma Yardımcısı.](https://aka.ms/SaRA_OfficeSCA_M365Portal) Office Dağıtım Aracı'nı kullanarak yüklemeleri özelleştirmeyle ilgili önkoşullar, kurulum yönergeleri ve yönergeler hakkında ayrıntılar için bkz. Uzak Masaüstü Hizmetleri'Microsoft 365 Uygulamaları kullanarak [yüklemeleri dağıtma](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Paylaşılan bilgisayar etkinleştirmesi ile ilgili hataları düzeltmek için bkz:

- [E-posta için paylaşılan bilgisayar etkinleştirme sorunlarını Microsoft 365 Uygulamaları](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Kuruluş etkinleştirme durumunu için Microsoft 365 Uygulamalarını sıfırlayın.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Microsoft 365 Uygulamaları'i varsayılan yükleme ayarlarını kullanan Microsoft 365 yönetim merkezi RDS'e yüklemek için aşağıdaki adımları izleyin:

1. Sahip Microsoft 365 planınız olduğunu kontrol edin. Daha fazla bilgi için [bkz. Hangi aboneliğe sahipim?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Gerekirse farklı bir plana Microsoft 365. Daha fazla bilgi için [bkz. Farklı bir plana yükseltme](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Başka Microsoft 365 Uygulamaları uyumsuz planları kullanarak RDS sunucusuna zaten yüklenmişse, Denetim Masası'nda Program   >  **kaldırma'ya gidip programı kaldırın.** Sorun olursa, [Microsoft Destek ve Kurtarma Yardımcısı'i indirerek](https://aka.ms/SARA-OfficeUninstall-Alchemy)kaldırın.

1. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetim merkezi oturum açın ve yükleme [Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Yükleme Office, herhangi bir uygulama açmayın veya Office açmayın.

1. RDS sunucusunda, paylaşılan bilgisayar etkinleştirmesini etkinleştirmek için kayıt defterini düzenleme:

   1. Ekranın sol alt Windows Seçenekler düğmesine sağ tıklayın ve Çalıştır'ı **seçin.** Aç kutusuna, **regedit** yazın ve sonra da **Tamam**'ı seçin.

   1. Kayıt Defteri Düzenleyicisi'nin aygıtınızda değişiklik yapmasına izin vermek istendiğinde Evet'i **seçin.**

   1. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration öğesinin altında, 1 ayarıyla **SharedComplicensing'in** dize **değerini ekleyin.**

1. RDS sunucusunda, son kullanıcı olarak oturum açma ve son kullanıcı için paylaşılan bilgisayar etkinleştirmenin etkinleştirildiğinden emin Microsoft 365 Uygulamaları. 

   Ayrıntılar için [bkz. Paylaşılan bilgisayar etkinleştirmenin Etkinleştirildiğinden emin Microsoft 365 Uygulamaları.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)