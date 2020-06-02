---
title: RDS, Terminal Server veya VDI'de paylaşılan kullanım için kurumsal olarak Microsoft 365 Uygulamalarını dağıtma
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507606"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS, Terminal Server veya VDI'de paylaşılan kullanım için kurumsal olarak Microsoft 365 Uygulamalarını dağıtma

Eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetlerini (RDS) kullanarak kurumsal kuruluş için Microsoft 365 Uygulamalarını dağıtmak için:
- Office 365 Enterprise E3 veya Enterprise E5 gibi kurumsal Microsoft 365 Uygulamaları içeren bir Microsoft 365 İş Için planı nız veya Office 365 planınız olmalıdır.
   > [!NOTE] 
   > Microsoft 365 İş Uygulamaları ve Microsoft 365 Business Premium Standart planları, kurumsal için Microsoft 365 Apps'ı içermez.
- [Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)etkinleştirmelisiniz.

> [!NOTE]
> Microsoft 365 Apps for enterprise'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) da indirip çalıştırabilirsiniz.

Office Dağıtım Aracı'nı kullanarak ön koşullar, kurulum yönergeleri ve özelleştirilmiş yüklemeler hakkında daha fazla bilgi için, [Uzak Masaüstü Hizmetlerini kullanarak Microsoft 365 Uygulamalarını kurumsal olarak dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)bakın.

Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:
- [Microsoft 365 Kurumsal Uygulamalar için paylaşılan bilgisayar etkinleştirme ile Sorun Giderme sorunlarına](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)bakın.
- Bkz. [Kuruluşlar için Microsoft 365 Uygulamaları etkinleştirme durumunu sıfırlama](https://go.microsoft.com/fwlink/?linkid=2109218).

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'de kurumsal olarak Microsoft 365 Uygulamaları yüklemek istiyorsanız, aşağıdaki adımları kullanın:

1.    Hangi aboneliğiniz olduğunu kontrol edin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Gerekirse, farklı bir aboneye geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Office, rds sunucusunda başka Microsoft abonelikleri kullanıyorsa, kaldırın. Örneğin, **Denetim Masası'na**giderek  >  **bir programı kaldırın.** Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.
4.    RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [kurumsal için Microsoft 365 Uygulamaları'nı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)
5.    Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***
6.    RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:
   1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve **Çalıştır'ı**seçin. Açık kutusunda **regedit**yazın ve ardından **Tamam'ı**seçin.
   2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde **Evet'i** seçin.
   3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.
   4. RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve microsoft [365 Kurumsal Uygulamalar için paylaşılan bilgisayar etkinleştirme etkinleştirme etkin olduğunu doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

