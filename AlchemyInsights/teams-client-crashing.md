---
title: Teams istemcisinin kilitlenmesi
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890358"
---
# <a name="teams-client-crashing"></a>Teams istemcisinin kilitlenmesi

Teams istemciniz kilitleniyorsa şunları deneyin:

- Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Tüm önemli [URL'Microsoft 365 erişilebilir olduğundan](https://docs.microsoft.com/microsoftteams/connectivity-issues) emin olun.

- Kiracı yönetici hesabınızla oturum açın ve kesinti [veya](https://docs.microsoft.com/office365/enterprise/view-service-health) hizmet performansında düşüş olmadığını doğrulamak için Hizmet Durumu Pano'nıza göz atabilirsiniz.

- Teams Uygulamasını kaldırma ve yeniden yükleme
    - Bilgisayarınızda %appdata%\Microsoft\Teams\ klasörüne gidin ve o dizindeki tüm dosyaları silin.
    - [Teams Uygulaması'Teams](https://www.microsoft.com/microsoft-teams/download-app)indirip yükleyin ve mümkünse yönetici olarak Teams yükleyin (Teams yükleyicisini sağ tıklatın ve varsa Yönetici olarak çalıştır'ı  seçin).

Teams istemciniz hala kilitlenmeye devam ediyorsa, sorunu yeniden oluşturmaya deneyin. Şunları biliyorsanız:

1. Adımlarınızı yakalamak için Adım Kaydedicisi'yi kullanın.
    - TÜM gereksiz veya gizli uygulamaları kapatın.
    - Etkilenen kullanıcı hesabıyla oturum açmış durumdayken Adım Kaydedicisi'ni başlatarak sorunu yeniden üretin.
    - [Kaydedilen yeniden proje adımlarını yakalayan ekip günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files) **Not:** Etki alanı etki olan kullanıcının oturum açma adresini yakalamayı unutmayın.
    - Dökümü ve/veya Hata demeti bilgilerini toplayın (Windows). Kilitlenme Windows makinede Powershell'i çalıştırın ve aşağıdaki komutları çalıştırın (her komuttan sonra Enter tuşuna basın):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Metin dosyası oluşturularak ekran üzerinde görüntülendiğinde, dosyayı kaydedin ve hizmet isteğine iliştirin. 
