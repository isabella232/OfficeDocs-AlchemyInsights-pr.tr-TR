---
title: Sorun Giderme OneDrive çöküyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749242"
---
# <a name="troubleshoot-onedrive-crashes"></a>Sorun Giderme OneDrive çöküyor

OneDrive sürekli olarak çöküyorsa, şu sorun giderme adımlarını deneyin:

**Kayıt defteri anahtarlarının ayarlı olmadığından emin olun:**

1. Kayıt Defteri Düzenleyicisi'ni kullanarak HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive'a gidin
2. DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak değiştirin.
3. Start'a giderek OneDrive'ı el ile başlatın ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

**OneDrive'ı Sıfırla:**

Notlar:

- OneDrive'ı sıfırlamak, mevcut eşitleme bağlantılarınızın bağlantısını keser (ayarlanmışsa kişisel OneDrive'ınız dahil).
- OneDrive'ı bilgisayarınızda sıfırlayarak dosya veya veri kaybetmezsiniz.

**OneDrive'ı sıfırlamak için:**

1. Windows tuşu ve R tuşuna basarak Çalıştır iletişim kutusunu açın.
2. %localappdata%\Microsoft\OneDrive\onedrive.exe /reset yazın ve Tamam tuşuna basın. Komut penceresi kısa bir süre görünebilir.
3. Start'a giderek OneDrive'ı el ile başlatın ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.

Notlar:

- Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiyseniz, eşitleme tamamlandıktan sonra bunu tekrar yapmanız gerekir. Daha fazla bilgi için [bilgisayarınızla eşitlenebilmek için hangi OneDrive klasörlerini](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   seç'i okuyun.
- Kişisel OneDrive ve OneDrive for Business için bunu tamamlamanız gerekir.