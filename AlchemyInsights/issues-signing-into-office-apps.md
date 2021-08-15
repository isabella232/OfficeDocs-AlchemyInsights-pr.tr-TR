---
title: Microsoft 365 uygulamalarda oturum açma sorunları
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986911"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Şu Microsoft 365 düzeltme "Bilgisayarınızın Güvenilen Platform modülü düzgün çalışmıyor" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Windows ve [Office](https://support.microsoft.com/help/4027667/windows-10-update) [için en son güncelleştirmeleri yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Kimlik Office Yöneticisi'ni kullanarak](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. (Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilir Platform [Modülü](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (TPM) hatalarını düzeltmek için kullanıcı kurtarma işlemini deneyin.
- Aşağıdaki adımları kullanarak EnableADAL = 0 ayarlayın:  
    1. Başlat düğmesine sağ tıklayın Windows Çalıştır'ı **seçin,** **regedit yazın ve** ardından Tamam'ı **seçin.**
    2. Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmalarına izin vermek için Evet'i seçin.
    3. Kayıt Defteri Düzenleyicisi'nde, Düzenleyici'nin altında **0** değeriyle **EnableADAL** için DWORD HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daha fazla bilgi için bkz. [Windows 10'de Office 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)derlemesi ile Office sonra oturum açma ile ilgili bağlantı Windows 10.