---
title: Bir Terminal sunucusunda - lisanssız Office yükleme
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498435"
---
# <a name="installing-office-on-a-terminal-server"></a>Office bir Terminal sunucusuna program yükleme

Uzak Masaüstü Hizmetleri (RDS) kullanan Windows Server Office 365 ProPlus dağıtmak için önceden Terminal Hizmetleri olarak adlandırılan:
  
- Office 365 ProPlus, Office 365 Kurumsal E3 veya Kurumsal E5 gibi içeren bir Office 365 planınız olmalıdır. Office 365 iş ve Office 365 iş Premium planları Office 365 ProPlus dahil etmeyin.

- [Paylaşılan bilgisayar](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmesi gerekir.

Office 365 portal, ***varsayılan yükleme ayarlarını kullanan***Office 365 ProPlus RDS yüklemek istiyorsanız şu adımları izleyin:
  
1. Elinizde hangi Office 365 planını denetleyin. [Öğrenin nasıl](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Gerekirse, başka bir Office 365 anahtarı düşünüyorsanız. [Öğrenin nasıl](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Diğer Office 365 planları kullanarak RDS Sunucu üzerinde Office yüklüyse, kaldırın. Örneğin, Denetim Masası'na giderek tarafından \> program Kaldır. Sorunlar çalıştırıyorsanız, [Microsoft destek ve kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.

4. RDS Sunucu üzerinde yönetici hesabı ve [Office 365 ProPlus yüklemek](https://portal.office.com/OLS/MySoftware.aspx)Office 365 portalına oturum açın.

5. Office yüklendikten sonra ***açmayın veya oturum açmak*** için herhangi bir Office uygulaması.

6. RDS Sunucu üzerinde aaıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirme etkinleştir:

1. Ekranın sol alt köşesinde Windows düğmesini sağ tıklatın ve Çalıştır'ı seçin. Aç kutusuna **regedit**yazın ve Tamam'ı seçin.

2. Evet, aygıtınız için değişiklik yapmak için Kayıt Defteri Düzenleyicisi'ni izin vermek isteyip istemediğiniz sorulduğunda seçin.

3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı ile **SharedComputerLicensing** bir dize değeri ekleyin.

7. RDS Sunucu, ***bir son kullanıcı oturum açın*** ve [paylaşılan bilgisayar etkinleştirme Office 365 ProPlus için etkinleştirilmiş olduğunu doğrulayın](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Önkoşullar, kurulum yönergelerini ve Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeleri Kılavuzu hakkında daha fazla ayrıntı için lütfen [Dağıtmak Office 365 Uzak Masaüstü Hizmetleri kullanarak ProPlus](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.
  
Paylaşılan bilgisayar etkinleştirme için ilgili hataları gidermek için [Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme ile ilgili sorunları giderme](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)konusuna bakın.
  