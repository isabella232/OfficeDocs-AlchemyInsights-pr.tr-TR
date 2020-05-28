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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354073"
---
# <a name="teams-client-crashing"></a>Teams istemcisi kilitleniyor mu?

Teams istemciniz kilitleniyorsa şunları deneyin:

- Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Tüm Microsoft [365 URL'lerine ve adres aralıklarına](https://docs.microsoft.com/microsoftteams/connectivity-issues) erişilebildiğinden emin olun.

- Kiracı yönetici hesabınızla oturum açın ve kesinti veya hizmet bozulması olmadığını doğrulamak için [Hizmet Durumu Panosunuzu](https://docs.microsoft.com/office365/enterprise/view-service-health) kontrol edin.

- Takım Uygulamasını kaldırın ve yeniden yükleyin (bağlantı)
    - Bilgisayarınızdaki %appdata%\Microsoft\teams\ klasörüne göz atın ve bu dizindeki tüm dosyaları silin.
    - [Takımlar Uygulamasını indirin ve yükleyin](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ve mümkünse Takımlar'ı yönetici olarak yükleyin (Takımlar yükleyicisini sağ tıklatın ve varsa "Yönetici olarak çalıştır"ı seçin).

Teams istemciniz hala çöküyorsa, sorunu yeniden oluşturabilirsiniz? Eğer öyleyse:

1. Adımlarınızı yakalamak için Steps Kaydedici'yi kullanın.
    - TÜM gereksiz veya gizli uygulamaları kapatın.
    - Steps Kaydedici'yi başlatın ve etkilenen kullanıcı hesabıyla oturum açtırırken sorunu yeniden üretin.
    - [Kaydedilen repro adımlarını yakalayan takım günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files) **Not**: Etkilenen kullanıcının oturum açma adresini yakaladığından emin olun.
    - Döküm ve/veya Hata kovası bilgilerini (Windows) toplayın. Windows Powershell'i çökmenin meydana geldiği makinede başlatın ve aşağıdaki komutları çalıştırın:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Dosyayı destek servis talebinize takın.
