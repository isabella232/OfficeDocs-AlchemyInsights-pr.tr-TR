---
title: RDS, Terminal Server veya VDI'de paylaşılan kullanım için Office 365 ProPlus'ı dağıtma
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959479"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS, Terminal Server veya VDI'de paylaşılan kullanım için Office 365 ProPlus'ı dağıtma

Office 365 ProPlus'ı, eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetlerini (RDS) kullanarak dağıtmak için:
- Bir Microsoft 365 İşletmeler İçin planınız veya Office 365 ProPlus içeren Office 365 Planı(Office 365 Enterprise E3 veya Enterprise E5 gibi) olmalıdır.
   > [!NOTE] 
   > Office 365 Business ve Office 365 Business Premium planları Office 365 ProPlus'ı içermez.
- [Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmelisiniz.

> [!NOTE]
> Office 365 ProPlus'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.

Office Dağıtım Aracı'nı kullanarak ön koşullar, kurulum talimatları ve özelleştirilmiş yüklemeler hakkında daha fazla bilgi için, [Uzak Masaüstü Hizmetlerini kullanarak Office 365 ProPlus'ı dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.

Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:
- [Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme siyle ilgili Sorun Giderme sorunlarına](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)bakın.
- Bkz. [Office 365 ProPlus etkinleştirme durumunu sıfırla.](https://go.microsoft.com/fwlink/?linkid=2109218)

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'ye Office 365 ProPlus'ı yüklemek istiyorsanız, aşağıdaki adımları kullanın:

1.  Hangi Office 365 planınız olup deiyi kontrol edin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Gerekirse, farklı bir Office 365 planına geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Office, diğer Office 365 planlarını kullanarak RDS sunucusuna zaten yüklüyse, kaldırın. Örneğin, **Denetim Masası'na** > giderek**bir programı kaldırın.** Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.
4.  RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [Office 365 ProPlus'ı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)
5.  Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***
6.  RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:
   1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve **Çalıştır'ı**seçin. Açık kutusunda **regedit**yazın ve ardından **Tamam'ı**seçin.
   2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde **Evet'i** seçin.
   3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.
   4. RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve Paylaşılan bilgisayar [etkinleştirme Office 365 ProPlus için etkinleştirildiğinden doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

