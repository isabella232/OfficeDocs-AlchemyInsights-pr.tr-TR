---
title: Office uygulamalarında oturum açma sorunları
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763021"
---
# <a name="issues-signing-in-to-office-apps"></a>Office uygulamalarında oturum açma sorunları

Office uygulamalarıyla ilgili oturum açma sorunlarını gidermek için aşağıdakileri deneyin:

- Windows Ayarları > **Access çalışmasını veya okul'u**kullanarak etkilenen hesap dışındaki tüm iş hesaplarını kaldırın.
- Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)<br/>
    **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. (Ör. \Software\Microsoft\Office\16.0\Common\Identity\)
- Office uygulaması açın, **Dosya** > **Hesabı** > **Oturum Aç'ı**seçin. Ardından geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz. [Office Mac 2016 uygulamasında oturum açılamıyor](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Office 2013'u kullanarak Microsoft 365'e bağlanırken hatalar oluşursa, Office istemcisi için modern kimlik doğrulamasını etkinleştirin.

Daha fazla bilgi için bkz.:
- [Microsoft 365, Azure veya Intune'da oturum açamam](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Office 2016'ya güncelleştirmeden sonra oturum açma sorunları Windows 10'da 16.0.7967 oluşturma](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [Office'te "Üzgünüz, kuruluşunuzdaki başka bir hesap zaten bu bilgisayarda oturum açmış"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [ADFS kullanırken Office modern kimlik doğrulamasıyla ilgili oturum açma sorunlarını giderme](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)