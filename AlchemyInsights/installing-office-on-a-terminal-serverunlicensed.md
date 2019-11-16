---
title: Terminal Sunucusuna ofis yükleme - Lisanssız
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205429"
---
# <a name="installing-office-on-a-terminal-server"></a>Terminal Sunucusuna Office Yükleme

Office 365 ProPlus'ı, eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetlerini (RDS) kullanarak bir Windows Server'da dağıtmak için:
  
- Office 365 ProPlus'ı içeren Office 365 planınız olmalıdır(Office 365 Enterprise E3 veya Enterprise E5). Office 365 Business ve Office 365 Business Premium planları Office 365 ProPlus'ı içermez.

- Paylaşılan bilgisayar [etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmeniz gerekir.

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'ye Office 365 ProPlus'ı yüklemek istiyorsanız, aşağıdaki adımları kullanın.

> [!TIP]
> Office 365 ProPlus'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.
  
1. Hangi Office 365 planınız olup deiyi kontrol edin. [Nasıl yapılacağını öğrenin](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Gerekirse, farklı bir Office 365 planına geçin. [Nasıl yapılacağını öğrenin](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Office, diğer Office 365 planlarını kullanarak RDS sunucusuna zaten yüklüyse, kaldırın. Örneğin, Denetim Masası'na \> giderek bir programı kaldırın. Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.

4. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [Office 365 ProPlus'ı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)

5. Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***

6. RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:

1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı seçin. Aç kutusunda **regedit**yazın ve ardından Tamam'ı seçin.

2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.

3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.

7. RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve Paylaşılan bilgisayar [etkinleştirme Office 365 ProPlus için etkinleştirildiğinden doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

Office Dağıtım Aracı'nı kullanarak ön koşullar, kurulum talimatları ve özelleştirilmiş yüklemelerle ilgili kılavuzlar hakkında daha fazla bilgi için lütfen [Uzak Masaüstü Hizmetlerini kullanarak Office 365 ProPlus'ı dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.
  
Paylaşılan bilgisayar etkinleştirmesiyle ilgili hataları gidermek [için, Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme sorunları bölümüne](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)bakın.
  