---
title: Office Uygulamalarını Düzeltme Hesabınız kötü bir durum iletisi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969891"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Office uygulamalarını düzeltme "Hesabınız kötü durumda" hatası

Bu hatayı düzeltmek için etkilenen bilgisayarda aşağıdaki seçenekleri deneyin:

- Bir Office uygulaması açın, tüm hesaplardan **Dosya** > **Hesabı** > **Oturum Aç'ı**seçin. Geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak yeniden oturum açın. Ayrıntılı bilgi için [Bkz. Ofis'teki Hesaplar.](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)
- Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)<br>
  **Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi. Örneğin, \Software\Microsoft\Office\16.0\Common\Identity\
- Etkilenen bilgisayarda Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:  
     1. Windows düğmesine sağ tıklayın ve **Çalıştır'ı**seçin. **Açık** kutusunda **regedit**yazın ve ardından **Tamam'ı**seçin.
     2. Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde **Evet'i** seçin.
    3. Kayıt Defteri Düzenleyicisi'nde, HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında 0 ayarı olan EnableADAL'ın DWORD değerini ekleyin.
- Office 2013'u kullanarak Office 365'e bağlanırken hata oluşursa, Office [istemcisi için modern kimlik doğrulamasını etkinleştirin.](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)

Daha fazla bilgi için, [Office 365, Azure veya Intune'da oturum açamayan tarayıcı dışı uygulamaların nasıl giderilene](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)bakınız.

