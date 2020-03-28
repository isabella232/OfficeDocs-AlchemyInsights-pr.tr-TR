---
title: Teams istemcisi kilitleniyor mu?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030760"
---
# <a name="teams-client-crashing"></a>Teams istemcisi kilitleniyor mu?

Teams istemciniz kilitleniyorsa şunları deneyin:

- Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Tüm [Office 365 URL’lerinin ve adres aralıklarının](https://docs.microsoft.com/microsoftteams/connectivity-issues) erişilebilir durumda olduğundan emin olun.

- Kesinti veya hizmet performansında düşüş olmadığından emin olmak için yönetici hesabınızla oturum açın ve [Hizmet Durumu Panonuzu](https://docs.microsoft.com/office365/enterprise/view-service-health) denetleyin.

 - Son olarak, Teams istemci önbelleğinizi temizlemeyi deneyebilirsiniz:

    1.  Microsoft Teams masaüstü istemcisinden tamamen çıkın. Simge Tepsisinden **Teams**’e sağ tıklayıp **Çık**’a tıklayabilir veya Görev Yöneticisi’ni çalıştırıp işlemi tamamen sonlandırabilirsiniz.

    2.  Dosya Gezgini’ne gidin ve %appdata%\Microsoft\teams yazın.

    3.  Dizine girdiğinizde şu klasörlerden birkaç tanesini görürsünüz:

         - **Uygulama Önbelleği** içinden Önbellek’e gidip Önbellek konumundaki (%appdata%\Microsoft\teams\application cache\cache) dosyalardan dilediğinizi silin.

        - **Blob_storage** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\blob_storage.

        - **Önbellek** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\Cache.

        - **Veritabanları** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\databases.

        - **GPUCache** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\GPUcache.

        - **IndexedDB** içindeki .db uzantılı dosyayı silin: %appdata%\Microsoft\teams\IndexedDB.

        - **Yerel Depolama** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\Local Storage.

        - Son olarak, **tmp** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\tmp.

    4. Teams istemcinizi yeniden başlatın.
