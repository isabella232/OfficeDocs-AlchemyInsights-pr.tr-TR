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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744666"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>E-Microsoft 365 Uygulamaları'da oturum açma sorunları

Not: Windows'ın eski bir sürümünü (örneğin, Windows 7 SP1, Windows Server 2008 R2) kullanıyorsanız, kolay düzeltmeyi kullanarak TLS 1.2'yi varsayılan olarak etkinleştirin. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için Windows.

Microsoft 365 Uygulamalarındaki oturum açma sorunlarını çözmek için, etkilenen makinede aşağıdaki seçenekleri deneyin:  

- Daha Windows için [bkz. Öneriler oturum açma sorunlarını çözme hakkında daha fazla bilgi](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Mac için [bkz. Office Mac 2016 uygulamasında Office Mac 2016.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**İpucu** Windows makinelerde sizin için birçok genel Office oturum açma sorunlarını tanılayabilir ve otomatik olarak düzeltebiliriz. Otomatik aracımızı kullanmak için  **[Office 365 Destek ve Kurtarma Yardımcısını](https://aka.ms/SaRA-OfficeSignInScenario)** indirip çalıştırın.

**Not:** Oturum açma veya etkinleştirme sorunlarını düzeltmek için Modern Kimlik Doğrulama (ADAL) veya Web Hesabı Yönetimi'ni (WAM) devre **dışı bırakmanız önerilmez.** Office 2013'ü kullanarak Microsoft 365 bağlanırken hata oluşursa, Office için [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) kimlik doğrulamayı etkinleştirmeye Office olun.

Belirli sorun giderme eylemleri için bkz:

[Windows 10'da, Office 2016 derleme 16.0.7967'ye güncelleştirmeden sonra oturum açmada bağlantı sorunları](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Office 365, Azure veya Intune gibi kuruluş hesabınızla oturum alayasınız](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Office 365, Azure veya Intune'da oturum açmayan tarayıcı olmayan uygulamaların sorunlarını giderme](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[E-postada arka arkaya kimlik Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)