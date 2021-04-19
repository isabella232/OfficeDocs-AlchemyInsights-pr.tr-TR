---
title: Teams istemcisi kilitleniyor mu?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826291"
---
# <a name="teams-client-crashing"></a>Teams istemcisi kilitleniyor mu?

Teams istemciniz kilitleniyorsa şunları deneyin:

- Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Tüm Microsoft [365 URL'leri ve adres aralıklarını erişilebilir olduğundan](https://docs.microsoft.com/microsoftteams/connectivity-issues) emin olun.

- Kiracı yönetici hesabınızla oturum açın ve kesinti [veya](https://docs.microsoft.com/office365/enterprise/view-service-health) hizmet performansında bir düşüş olmadığını doğrulamak için Hizmet Durumu Pano'nıza göz atabilirsiniz.

- Teams Uygulamasını kaldırma ve yeniden yükleme (bağlantı)
    - Bilgisayarınızda %appdata%\Microsoft\teams\ klasörüne gidin ve bu dizindeki tüm dosyaları silin.
    - [Teams Uygulamasını indirip yükleyin ve](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)mümkünse Teams'i yönetici olarak yükleyin (Teams yükleyicisi'ne sağ tıklayın ve varsa "Yönetici olarak çalıştır"ı seçin).

Teams istemciniz hala kilitlenmeye devam ediyorsa sorunu yeniden ürete misiniz? Öyleyse:

1. Adımlarınızı yakalamak için Adım Kaydedicisi'yi kullanın.
    - TÜM gereksiz veya gizli uygulamaları kapatın.
    - Etkilenen kullanıcı hesabıyla oturum açmış durumdayken Adım Kaydedicisi'ni başlatarak sorunu yeniden üretin.
    - [Kaydedilen yeniden proje adımlarını yakalayan ekip günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files) **Not:** Etki alanı etki olan kullanıcının oturum açma adresini yakalamayı unutmayın.
    - Dökümü ve/veya Hata demeti bilgilerini (Windows) toplayın. Kilitlenmenin olduğu makinede Windows Powershell'i çalıştırın ve aşağıdaki komutları çalıştırın:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Dosyayı destek olaynıza iliştirin.
