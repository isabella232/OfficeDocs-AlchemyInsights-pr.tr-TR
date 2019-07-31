---
title: Office uygulamaları için oturum açma sorunları
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938376"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Office uygulamaları "bilgisayarınızın Güvenilen Platform Modülü düzgün çalışmıyor" iletisini çözme

Bu hatayı düzeltmek için aşağıdakileri deneyin:

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile ilgili en son güncelleştirmeleri yükleyin.
- Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Güvenilir Platform Modülü (TPM) hataları düzeltmek için [kullanıcı kurtarma işlemi](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.
- Set EnableADAL = 0 aşağıdaki adımları kullanarak:  
    1. Windows Başlat düğmesini sağ tıklatın, **Çalıştır**' ı seçin, **regedit**yazın ve **Tamam**' ı seçin.
    2. Kayıt Defteri Düzenleyicisi, aygıtınız için değişiklik yapmak için izin vermek için **Evet** ' i seçin.
    3. Kayıt Defteri Düzenleyicisi'nde bir ayarı **0** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında **EnableADAL** DWORD değerini ekleyin.

Daha fazla bilgi için bkz: [oturum bileşeninde Office 2016 yapı 16.0.7967 Windows 10 üzerinde güncelleştirme sonra bağlantı sorunları](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).