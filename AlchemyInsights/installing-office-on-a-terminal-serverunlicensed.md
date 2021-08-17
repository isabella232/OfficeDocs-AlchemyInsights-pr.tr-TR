---
title: Terminal Sunucusuna ofis yükleme - Lisanssız
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055178"
---
# <a name="installing-office-on-a-terminal-server"></a>Terminal Office'ne yükleme

Uzak Masaüstü Kurumlar için Microsoft 365 Uygulamaları (RDS) Windows Terminal Hizmetleri'ni (RDS) kullanarak bir Windows Sunucusu üzerinde dağıtım için:
  
- E3 veya Microsoft 365 E5 gibi Kurumlar için Microsoft 365 Uygulamaları içeren bir Office 365 Kurumsal aboneliğiniz Enterprise gerekir. Proje İş için Microsoft 365 Uygulamaları İş için Microsoft 365 Uygulamaları Premium planlarına proje Kurumlar için Microsoft 365 Uygulamaları.

- Paylaşılan bilgisayar [etkinleştirmeyi etkinleştirmeniz gerekir.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Varsayılan yükleme ayarlarını kullanan Kurumlar için Microsoft 365 Uygulamaları RDS'Microsoft 365 yönetim merkezi rds üzerine yüklemek için aşağıdaki adımları kullanın.

> [!TIP]
> Ayrıca, paylaşılan bilgisayar etkinleştirme modunda Destek ve Kurtarma Yardımcısı [için Microsoft Kurumlar için Microsoft 365 Uygulamaları'ni](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.
  
1. Hangi Microsoft 365 sahip olduğunu kontrol edin. [Nasıl olduğunu öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Gerekirse farklı bir kullanıcı aboneliğine Microsoft 365 geçin. [Nasıl olduğunu öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Office diğer abonelikler kullanılarak RDS sunucusuna zaten Microsoft 365 varsa, bu aboneliği kaldırın. Örneğin, Denetim Masası'nı Kullanarak \> Programı kaldır'ı seçin. Sorun [Destek ve Kurtarma Yardımcısı](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft Destek ve Kurtarma Yardımcısı'ı kullanarak programı kaldırın.

4. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetim merkezi oturum açın ve yükleme [Kurumlar için Microsoft 365 Uygulamaları.](https://portal.office.com/OLS/MySoftware.aspx)

5. Yükleme Office, herhangi bir ***uygulama açmayın veya Office*** açın.

6. RDS sunucusunda, aşağıdaki adımları takip edin ve kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:

1. Ekranın sol alt Windows Seçenekler düğmesine sağ tıklayın ve Çalıştır'ı seçin. Aç kutusuna **regedit yazın ve** Tamam'ı seçin.

2. Kayıt Defteri Düzenleyicisi'nin aygıtınızda değişiklik yapmaya izin vermesine izin vermek istendiğinde Evet'i seçin.

3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarıyla **SharedCompcomplicensing** dize değeri ekleyin.

7. RDS sunucusunda, son ***kullanıcı olarak oturum açma ve*** son kullanıcı için paylaşılan bilgisayar [etkinleştirmenin etkinleştirildiğinden emin Kurumlar için Microsoft 365 Uygulamaları.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Önkoşullar, kurulum yönergeleri ve Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeler ile ilgili yönergeler ve yönergeler için bkz. Uzak Masaüstü Hizmetleri kullanarak [Kurumlar için Microsoft 365 Uygulamaları'i dağıtma.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Paylaşılan bilgisayar etkinleştirmesi ile ilgili hataları düzeltmek için lütfen Paylaşılan bilgisayarda etkinleştirmeyle ilgili sorunları giderme [Kurumlar için Microsoft 365 Uygulamaları.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  