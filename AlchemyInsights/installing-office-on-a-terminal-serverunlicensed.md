---
title: Office 'i Terminal sunucusuna yükleme-lisanssız
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663137"
---
# <a name="installing-office-on-a-terminal-server"></a>Office 'i Terminal sunucusuna yükleme

Windows Server 'da kurumsal olarak Microsoft 365 uygulamalarını dağıtmak için, eski adıyla Terminal Hizmetleri adlı uzak Masaüstü Hizmetleri (RDS) kullanın:
  
- Office 365 Kurumsal E3 veya Kurumsal E5 gibi kuruluş için Microsoft 365 uygulamalarını içeren bir Microsoft 365 aboneliğiniz olmalıdır. İş için Microsoft 365 uygulamaları ve Microsoft 365 Uygulamaları İş Ekstra planları için Microsoft 365 uygulamaları bulunmaz.

- [Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)etkinleştirmeniz gerekir.

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 Yönetim merkezinden kuruluş için Microsoft 365 uygulamalarını yüklemek istiyorsanız, aşağıdaki adımları kullanın.

> [!TIP]
> Paylaşılan bilgisayar etkinleştirme modu 'nda kuruluş için Microsoft 365 uygulamalarını yüklemek üzere [Microsoft destek ve Kurtarma Yardımcısı](https://aka.ms/SaRA_OfficeSCA_M365Portal) 'nı indirebilir ve çalıştırabilirsiniz.
  
1. Sahip olduğunuz Microsoft 365 aboneliğini denetleyin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Gerekirse, farklı bir Microsoft 365 aboneliğine geçin. [Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Office, başka bir Microsoft 365 aboneliğini kullanarak RDS sunucusunda zaten yüklüyse kaldırın. Örneğin, Denetim Masası 'Ndan \> bir program Kaldır 'a giderek. Sorun yaşıyorsanız [Microsoft destek ve Kurtarma Yardımcısı 'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.

4. RDS sunucusunda, Yönetici hesabınızla Microsoft 365 Yönetim Merkezi 'nde oturum açın ve [Kurumsal Için microsoft 365 uygulamalarını yükleyin](https://portal.office.com/OLS/MySoftware.aspx).

5. Office yüklendikten sonra, hiçbir Office uygulamasında ***açmayın veya oturum açmayın*** .

6. RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:

1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve sonra da Run 'ı seçin. Aç kutusuna **Regedit**yazın ve Tamam 'ı seçin.

2. Kayıt Defteri Düzenleyicisi 'nin cihazınızda değişiklik yapmasına izin vermeniz istendiğinde Evet 'ı seçin.

3. Kayıt Defteri Düzenleyicisi 'nde, HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\clicktorun\configurationaltında 1 ayarına sahip **Sharedcomputerlicensing** dize değerini ekleyin.

7. RDS sunucusunda ***Son Kullanıcı olarak oturum açın*** ve [paylaşılan bilgisayar etkinleştirmenin Kurumsal Microsoft 365 uygulamaları için etkinleştirildiğini doğrulayın](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Önkoşullar hakkında daha fazla bilgi için, Office dağıtım Aracı kullanılarak özelleştirilmiş yüklemelerde [Microsoft 365 uygulamalarını dağıtma](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)konusuna bakın.
  
Paylaşılan bilgisayar etkinleştirme ile ilgili hataları düzeltmek için, lütfen [Enterprise Için Microsoft 365 uygulamalarında paylaşılan bilgisayar etkinleştirme sorunlarını giderme](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)konusuna bakın.
  