---
title: OneDrive kilitlenme sorunlarını giderme
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826219"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive kilitlenme sorunlarını giderme

OneDrive art arda kilitlenirse şu sorun giderme adımlarını deneyin:

**Kayıt defteri anahtarlarının ayarlanmay olduğundan emin olun:**

1. Kayıt Defteri Düzenleyicisi'ni kullanarak Kayıt Defteri'HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak ayarlayın.
3. Başlat'a gidip OneDrive'ı el ile başlatma ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)yazın, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

**OneDrive'ı sıfırlama:**

Notlar:

- OneDrive'ı sıfırlayarak mevcut tüm eşitleme bağlantılarınızı (ayarlanmışsa kişisel OneDrive dahil) bağlantısını kesebilirsiniz.
- Bilgisayarınızda OneDrive'ı sıfırlayarak dosyalarınız veya verileriniz kaybetmezsiniz.

**OneDrive'ı sıfırlamak için:**

1. Windows tuşu ve R tuşuna basarak Çalıştır iletişim kutusunu açın.
2. %localappdata%\Microsoft\OneDrive\onedrive.exe /reset yazın ve Tamam'a basın. Kısa süreli olarak bir Komut penceresi görünebilir.
3. Başlat'a gidip OneDrive'ı el ile başlatma ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)yazın, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

Notlar:

- Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiysanız, eşitleme tamamlandıktan sonra bunu yeniden eşitlemeniz gerekir. Daha [fazla bilgi için Hangi OneDrive klasörlerinin bilgisayarınıza eşitleneceklerini](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)seçme   makalesi'ni okuyun.
- Bunu kişisel OneDrive ve OneDrive İş için tamamlamanız gerekir.