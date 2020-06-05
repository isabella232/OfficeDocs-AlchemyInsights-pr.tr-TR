---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579885"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 uygulamalarını düzeltme "Bilgisayarınızın Güvenilir Platform modülü düzgün çalışmıyor" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)için en son güncelleştirmeleri yükleyin.
- Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. (Ör. \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilir Platform Modülü (TPM) hatalarını düzeltmek için [kullanıcı kurtarma işlemini](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.
- Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:  
    1. Windows Başlat düğmesine sağ tıklayın, **Çalıştır'ı**seçin, **regedit**yazın ve ardından **Tamam'ı**seçin.
    2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek için **Evet'i** seçin.
    3. Kayıt Defteri Düzenleyicisi'nde, HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında **0** ayarı olan **EnableADAL'ın** DWORD değerini ekleyin.

Daha fazla bilgi için bkz: [Windows 10'da Office 2016'da 16.0.7967'yi oluştur'a güncellemeden sonra oturum açma](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)bağlantısı sorunları.