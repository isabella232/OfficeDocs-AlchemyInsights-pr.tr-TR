---
title: Microsoft 365 uygulamalarında oturum açma sorunları
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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695199"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 uygulamalarının "bilgisayarınızın Güvenilir Platform Modülü düzgün çalışmıyor" iletisini Düzeltme

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- En son [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)güncelleştirmelerini yükleyin.
- Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir. (Örn: \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilir Platform Modülü (TPM) hatalarını düzeltmek için [Kullanıcı kurtarma işlemini](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.
- Aşağıdaki adımları kullanarak EnableADAL = 0 değerini ayarlayın:  
    1. Windows Başlat düğmesine sağ **tıklayın, Başlat 'ı seçin,** **Regedit**yazın ve **Tamam**'ı seçin.
    2. Kayıt Defteri Düzenleyicisi 'nin cihazınızda değişiklik yapmasına izin vermek için **Evet 'i** seçin.
    3. Kayıt Defteri Düzenleyicisi 'nde, HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity. altındaki **0** ayarına sahip **ENABLEADAL** DWORD değerini ekleyin

Daha fazla bilgi için, [Windows 10 ' da Office 2016 derleme 16.0.7967 güncelleştirmeden sonra oturum açma 'Daki bağlantı sorunlarını](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)izleyin.