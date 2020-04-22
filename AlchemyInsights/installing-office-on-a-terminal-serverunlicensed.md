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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763237"
---
# <a name="installing-office-on-a-terminal-server"></a>Terminal Sunucusuna Office Yükleme

Eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetleri 'ni (RDS) kullanarak Windows Server'da kurumsal olarak Microsoft 365 Uygulamaları dağıtmak için:
  
- Office 365 Enterprise E3 veya Enterprise E5 gibi kurumsal microsoft 365 Uygulamalarını içeren bir Microsoft 365 aboneliğiniz olmalıdır. Microsoft 365 İş Uygulamaları ve Microsoft 365 İş Premium planları için Uygulamalar, kurumsal için Microsoft 365 Apps'ı içermez.

- Paylaşılan bilgisayar [etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmeniz gerekir.

***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'de kurumsal olarak Microsoft 365 Uygulamaları yüklemek istiyorsanız, aşağıdaki adımları kullanın.

> [!TIP]
> Microsoft 365 Apps for enterprise'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) da indirip çalıştırabilirsiniz.
  
1. Hangi Microsoft 365 aboneliğine sahip olduğunuzu kontrol edin. [Nasıl yapılacağını öğrenin](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Gerekirse, farklı bir Microsoft 365 aboneliğine geçin. [Nasıl yapılacağını öğrenin](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Office, rds sunucusunda başka microsoft 365 abonelikleri kullanıyorsa, kaldırın. Örneğin, Denetim Masası'na \> giderek bir programı kaldırın. Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.

4. RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [kurumsal için Microsoft 365 Uygulamaları'nı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)

5. Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***

6. RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:

1. Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı seçin. Aç kutusunda **regedit**yazın ve ardından Tamam'ı seçin.

2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.

3. Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.

7. RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve microsoft [365 Kurumsal Uygulamalar için paylaşılan bilgisayar etkinleştirme etkinleştirme etkin olduğunu doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemelerle ilgili ön koşullar, kurulum talimatları ve kılavuzlar hakkında daha fazla bilgi için lütfen [Uzak Masaüstü Hizmetlerini kullanarak Microsoft 365 Uygulamalarını kurumsal olarak dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.
  
Paylaşılan bilgisayar etkinleştirmesiyle ilgili hataları gidermek için lütfen [Microsoft 365 Apps for enterprise için paylaşılan bilgisayar etkinleştirme sorunları bölümüne](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)bakın.
  