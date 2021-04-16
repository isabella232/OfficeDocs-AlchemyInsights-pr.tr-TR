---
title: Microsoft 365 uygulamalarını düzeltme Hesabınız kötü durumda
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812556"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 uygulamaları "Hesabınız kötü durumda" hatasını düzeltme

Bu hatayı düzeltmek için, etkilenen bilgisayarda aşağıdaki seçenekleri deneyin:

- Bir Office uygulamasını açın, Tüm  >  **hesapların Dosya Hesabı** Oturum  >  **Açma'sını seçin.** Geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak yeniden oturum açın. Ayrıntılı bilgi için bkz. [Office’te Hesaplar](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.<br>
  **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti. Örneğin, \Software\Microsoft\Office\16.0\Common\Identity\
- Office 2013'ü kullanarak Office 365'e bağlanırken hata oluşursa, Office istemcisi için [modern kimlik](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) doğrulamayı etkinleştirin.

Daha fazla bilgi için [bkz. Microsoft 365, Azure veya Intune'da](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)oturum alamayan tarayıcı olmayan uygulamaların sorunlarını giderme.

