---
title: OneDrive kilitleniyor sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665018"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive kilitleniyor sorunlarını giderme

OneDrive sürekli kilitleniyor, şu sorun giderme adımlarını deneyin:

**Kayıt defteri anahtarlarının ayarlanmadığından emin olun:**

1. Kayıt Defteri Düzenleyicisi 'ni kullanarak HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak değiştirin.
3. Başlat 'a giderek OneDrive 'ı el ile başlatın ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

**OneDrive 'ı sıfırlayın:**

Notlarında

- OneDrive 'ı sıfırlamak, var olan tüm eşitleme bağlantılarınızı (ayarlanmış olan kişisel OneDrive 'ı dahil) bağlantıyı keser.
- Bilgisayarınızda OneDrive 'ı sıfırlayarak dosyaları veya verileri kaybetmezsiniz.

**OneDrive 'ı sıfırlamak için:**

1. Windows tuşuna ve R tuşuna basarak bir Run iletişim kutusunu açın.
2. % LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset yazın ve Tamam 'a basın. Kısaca bir komut penceresi görüntülenebilir.
3. Başlat 'a giderek OneDrive 'ı el ile başlatın ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

Notlarında

- Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiyseniz, eşitleme tamamlandığında bunu yeniden yapmalısınız. Daha fazla bilgi için [hangi OneDrive klasörlerinin bilgisayarınıza eşitleneceğini seçin](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Kişisel OneDrive ve OneDrive Iş için bunu tamamlamanız gerekir.