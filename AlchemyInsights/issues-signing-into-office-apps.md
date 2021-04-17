---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833035"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 uygulamaları "Bilgisayarınızın Güvenilen Platform modülü düzgün çalışmıyor" iletisi düzeltme

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Windows ve Office için en [son güncelleştirmeleri](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. (Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilir Platform [Modülü](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (TPM) hatalarını düzeltmek için kullanıcı kurtarma işlemini deneyin.
- Aşağıdaki adımları kullanarak EnableADAL = 0 ayarlayın:  
    1. Windows Başlat düğmesine sağ tıklayın, Çalıştır'ı **seçin,** **regedit yazın ve** ardından Tamam'ı **seçin.**
    2. Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmalarına izin vermek için Evet'i seçin.
    3. Kayıt Defteri Düzenleyicisi'nde, Düzenleyici'nin altında **0** değeriyle **EnableADAL** için DWORD HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daha fazla bilgi için [bkz. Windows 10 üzerinde Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirdikten sonra oturum açma işlemiyle ilgili bağlantı sorunları.