---
title: Şirket için Microsoft 365 uygulamalarını RDS, Terminal Server veya VDı 'ta paylaşılan kullanıma yönelik olarak dağıtma
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786297"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Şirket için Microsoft 365 uygulamalarını RDS, Terminal Server veya VDı 'ta paylaşılan kullanıma yönelik olarak dağıtma

Daha önce Terminal Hizmetleri adlı uzak Masaüstü Hizmetleri (RDS) kullanarak Microsoft 365 uygulamalarını kurumsal dağıtmak için:
- Office 365 Kurumsal E3 veya Kurumsal E5 gibi Işletmeler için Microsoft 365 uygulamaları içeren bir Microsoft 365 Iş planı veya Office 365 planınız olmalıdır.
   > [!NOTE] 
   > İş için Microsoft 365 uygulamaları ve Microsoft 365 Iş ekstra standart planları kurumsal için Microsoft 365 uygulamaları içermez.
- [Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)etkinleştirmelisiniz.

> [!NOTE]
> Paylaşılan bilgisayar etkinleştirme modu 'nda kuruluş için Microsoft 365 uygulamalarını yüklemek üzere [Microsoft destek ve Kurtarma Yardımcısı](https://aka.ms/SaRA_OfficeSCA_M365Portal) 'nı indirebilir ve çalıştırabilirsiniz.

Office dağıtım Aracı kullanılarak özelleştirilmiş yüklemelerde Önkoşullar, kurulum yönergeleri ve yönergeler hakkında daha fazla bilgi için, [Uzak Masaüstü Hizmetleri 'ni kullanarak kurumsal Için Microsoft 365 uygulamalarını dağıtma](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)konusuna bakın.

Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:
- [Kurumsal Için Microsoft 365 uygulamalarında paylaşılan bilgisayar etkinleştirme sorunlarını giderme](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)konusuna bakın.
- Bkz. [Kuruluşlar için Microsoft 365 Uygulamaları etkinleştirme durumunu sıfırlama](https://go.microsoft.com/fwlink/?linkid=2109218).

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 Yönetim merkezinden kuruluş için Microsoft 365 uygulamalarını yüklemek istiyorsanız, aşağıdaki adımları kullanın:

1.    Sahip olduğunuz aboneliği denetleyin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Gerekirse, farklı bir aboneliğe geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Office, başka herhangi bir Microsoft aboneliğini kullanarak RDS sunucusunda zaten yüklüyse kaldırın. Örneğin, **Denetim Masası 'ndan**  >  **bir program Kaldır**'a giderek. Sorun yaşıyorsanız [Microsoft destek ve Kurtarma Yardımcısı 'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.
4.    RDS sunucusunda, Yönetici hesabınızla Microsoft 365 Yönetim Merkezi 'nde oturum açın ve [Kurumsal Için microsoft 365 uygulamalarını yükleyin](https://portal.office.com/OLS/MySoftware.aspx).
5.    Office yüklendikten sonra, hiçbir Office uygulamasında ***açmayın veya oturum açmayın*** .
6.    RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:
   1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve sonra da **Run**'ı seçin. Aç kutusuna **Regedit**yazın ve **Tamam 'ı**seçin.
   2. Kayıt Defteri Düzenleyicisi 'nin cihazınızda değişiklik yapmasına izin vermeniz istendiğinde **Evet 'i** seçin.
   3. Kayıt Defteri Düzenleyicisi 'nde, HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\clicktorun\configurationaltında 1 ayarına sahip **Sharedcomputerlicensing** dize değerini ekleyin.
   4. RDS sunucusunda ***Son Kullanıcı olarak oturum açın*** ve [paylaşılan bilgisayar etkinleştirmenin Kurumsal Microsoft 365 uygulamaları için etkinleştirildiğini doğrulayın](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

