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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938374"
---
# <a name="issues-signing-in-to-office-apps"></a>Office uygulamaları için oturum açma sorunları

Office uygulamaları ile oturum açma sorunlarını düzeltmek için aşağıdakileri deneyin:

- Windows ayarları > **erişim iş veya Okul**kullanarak etkilenen hesabı dışındaki tüm çalışma hesapları kaldırın.
- Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Bir Office uygulamasını açın, **Dosya** > **Hesap** > **Oturumu Kapat**. Sonra geçerli bir lisansa bir kullanıcı hesabı kullanarak oturum açın. Ayrıntılı bilgi için bkz: [Office hesapları](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac için bkz: [Mac app için bir Office 2016'da oturum açamıyorsunuz](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Hatalar oluşursa, Office kullanarak Office 2013 365 bağlanırken, Office istemcisi için modern kimlik doğrulamasını etkinleştirin.

Daha fazla bilgi için bkz.
- [Office 365, Azure veya Intune oturum açamıyorum](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Oturum açmak için Office 2016 güncelleştirmeden sonra bağlantı sorunları 16.0.7967 Windows 10 üzerinde oluşturun.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Üzgünüm, kuruluşunuzda başka bir hesaptan zaten imzalanan bu bilgisayar üzerinde" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [ADFS kullandığınızda Office modern kimlik doğrulamasıyla oturum sorunlarını giderme](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)