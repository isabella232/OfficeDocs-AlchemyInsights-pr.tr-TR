---
title: Teams kilitlenmesi
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321645"
---
# <a name="teams-client-crashing"></a>Teams kilitlenmesi

Teams istemciniz kilitleniyorsa şunları deneyin:

- Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Tüm url'lerin [Microsoft 365 erişilebilir olduğundan](https://docs.microsoft.com/microsoftteams/connectivity-issues) emin olun.

- Kiracı yönetici hesabınızla oturum açın ve kesinti [veya](https://docs.microsoft.com/office365/enterprise/view-service-health) hizmet performansında düşüş olmadığını doğrulamak için Hizmet Durumu Pano'nıza göz atabilirsiniz.

- Teams Uygulamasını kaldırma ve yeniden yükleme
    - Bilgisayarınızda %appdata%\Microsoft\Teams\ klasörüne gidin ve bu dizindeki tüm dosyaları silin.
    - [Teams Uygulamasını indirip yükleyin](https://www.microsoft.com/microsoft-teams/download-app)ve mümkünse Teams olarak yükleyin (Teams yükleyicisini sağ tıklatın ve varsa yönetici olarak **çalıştır'ı** seçin).

Teams istemciniz hala kilitlenmeye devam ediyorsa, sorunu yeniden oluşturmaya deneyin. Şunları biliyorsanız:

1. Adımlarınızı yakalamak için Adım Kaydedicisi'yi kullanın.
    - TÜM gereksiz veya gizli uygulamaları kapatın.
    - Etkilenen kullanıcı hesabıyla oturum açmış durumdayken Adım Kaydedicisi'ni başlatarak sorunu yeniden üretin.
    - [Kaydedilen yeniden proje adımlarını yakalayan ekip günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **Not:** Etki alanı etki olan kullanıcının oturum açma adresini yakalamayı unutmayın.
    - Dökümü ve/veya Hata demeti bilgilerini toplayın (Windows). Kilitlenme Windows makinede Powershell'i çalıştırın ve aşağıdaki komutları çalıştırın (her komuttan sonra Enter tuşuna basın):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Metin dosyası oluşturularak ekran üzerinde görüntülendiğinde, dosyayı kaydedin ve hizmet isteğine iliştirin. 
