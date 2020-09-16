---
title: Microsoft 365 uygulamalarını düzeltme hesabınız hatalı bir durumda
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744565"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 uygulamalarının "hesabınız hatalı bir durumda

Bu hatayı düzeltmek için etkilenen bilgisayarda aşağıdaki seçenekleri deneyin:

- Bir Office uygulamasını açın, **Dosya**  >  **hesabı**'nı  >  **Tüm hesaplarda oturumu Kapat**'ı seçin. Geçerli lisansa sahip bir kullanıcı hesabını kullanarak yeniden oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br>
  **Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir. Örneğin, \Software\Microsoft\Office\16.0\Common\Identity\
- Office 2013 kullanarak Office 365 ' a bağlanırken hata oluşursa, Office istemcisinde [modern kimlik doğrulamasını etkinleştirin](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) .

Daha fazla bilgi için, [Microsoft 365, Azure veya Intune 'da oturum açmayan tarayıcı olmayan uygulamalarda nasıl sorun giderileceği](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)bölümüne bakın.

