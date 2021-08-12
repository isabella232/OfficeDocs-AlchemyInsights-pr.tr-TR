---
title: OneDrive sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921027"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive sorunlarını giderme

Sürekli OneDrive kilitlenirse, şu sorun giderme adımlarını deneyin:

**Kayıt defteri anahtarlarının ayarlanmay olduğundan emin olun:**

1. Kayıt Defteri Düzenleyicisi'ni kullanarak Kayıt Defteri'HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak ayarlayın.
3. Başlat'OneDrive gidip el ile başlat ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)yazın OneDrive yazın ve Masaüstü uygulamasını OneDrive tıklayın.

**Parolayı OneDrive:**

Notlar:

- Ayarların OneDrive mevcut tüm eşitleme bağlantılarınızı (ayarlanmışsa kişisel eşitleme OneDrive bağlantısını keser).
- Bilgisayarınıza verilerinizi ya da dosyalarınızı ya da verilerinizi OneDrive kaybetmezsiniz.

**Parolayı sıfırlamak OneDrive:**

1. Windows ve R tuşlarına basarak Çalıştır iletişim kutusunu açın.
2. %localappdata%\Microsoft\OneDrive\onedrive.exe /reset yazın ve Tamam'a basın. Kısa süreli olarak bir Komut penceresi görünebilir.
3. Başlat'OneDrive gidip el ile başlat ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)yazın OneDrive yazın ve Masaüstü uygulamasını OneDrive tıklayın.

Notlar:

- Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiysanız, eşitleme tamamlandıktan sonra bunu yeniden eşitlemeniz gerekir. Daha [fazla OneDrive için Hangi klasörlerin bilgisayarınızla eşit okuy](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)salt okunur olduğunu   seçme.
- Bu işlemi kişisel bilgileriniz ve iş bilgileriniz için OneDrive OneDrive İş.