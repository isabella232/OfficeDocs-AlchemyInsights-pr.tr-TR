---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709126"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 uygulamalarını düzeltme "Bilgisayarınızın Güvenilen Platform modülü düzgün çalışmıyor" iletisi

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- Windows ve Office'in en [son güncelleştirmelerini](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilen Platform [Modülü](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (TPM) hatalarını düzeltmek için kullanıcı kurtarma işlemini deneyin.
- Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:  
    1. Windows Başlat düğmesine sağ tıklayın, Çalıştır'ı **seçin,** **regedit yazın** ve Tamam'ı **seçin.**
    2. Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmalarına izin vermek için Evet'i seçin.
    3. Kayıt Defteri Düzenleyicisi'nde, **0** ayarıyla **EnableADAL'ın** DWORD değerini HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daha fazla bilgi için, [Windows 10'da Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirme sonrasında oturum açmayla ilgili bağlantı sorunlarına bakın.