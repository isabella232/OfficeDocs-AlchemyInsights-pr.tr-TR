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
# <a name="teams-client-crashing"></a><span data-ttu-id="9ebdc-102">Teams istemcisi kilitleniyor mu?</span><span class="sxs-lookup"><span data-stu-id="9ebdc-102">Teams client crashing?</span></span>

<span data-ttu-id="9ebdc-103">Teams istemciniz kilitleniyorsa şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="9ebdc-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="9ebdc-104">Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9ebdc-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="9ebdc-105">Tüm Microsoft [365 URL'lerine ve adres aralıklarına](https://docs.microsoft.com/microsoftteams/connectivity-issues) erişilebildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="9ebdc-106">Kiracı yönetici hesabınızla oturum açın ve kesinti veya hizmet bozulması olmadığını doğrulamak için [Hizmet Durumu Panosunuzu](https://docs.microsoft.com/office365/enterprise/view-service-health) kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="9ebdc-107">Takım Uygulamasını kaldırın ve yeniden yükleyin (bağlantı)</span><span class="sxs-lookup"><span data-stu-id="9ebdc-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="9ebdc-108">Bilgisayarınızdaki %appdata%\Microsoft\teams\ klasörüne göz atın ve bu dizindeki tüm dosyaları silin.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="9ebdc-109">[Takımlar Uygulamasını indirin ve yükleyin](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ve mümkünse Takımlar'ı yönetici olarak yükleyin (Takımlar yükleyicisini sağ tıklatın ve varsa "Yönetici olarak çalıştır"ı seçin).</span><span class="sxs-lookup"><span data-stu-id="9ebdc-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="9ebdc-110">Teams istemciniz hala çöküyorsa, sorunu yeniden oluşturabilirsiniz?</span><span class="sxs-lookup"><span data-stu-id="9ebdc-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="9ebdc-111">Eğer öyleyse:</span><span class="sxs-lookup"><span data-stu-id="9ebdc-111">If so:</span></span>

1. <span data-ttu-id="9ebdc-112">Adımlarınızı yakalamak için Steps Kaydedici'yi kullanın.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="9ebdc-113">TÜM gereksiz veya gizli uygulamaları kapatın.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="9ebdc-114">Steps Kaydedici'yi başlatın ve etkilenen kullanıcı hesabıyla oturum açtırırken sorunu yeniden üretin.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="9ebdc-115">[Kaydedilen repro adımlarını yakalayan takım günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="9ebdc-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="9ebdc-116">**Not**: Etkilenen kullanıcının oturum açma adresini yakaladığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="9ebdc-117">Döküm ve/veya Hata kovası bilgilerini (Windows) toplayın.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="9ebdc-118">Windows Powershell'i çökmenin meydana geldiği makinede başlatın ve aşağıdaki komutları çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9ebdc-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="9ebdc-119">Dosyayı destek servis talebinize takın.</span><span class="sxs-lookup"><span data-stu-id="9ebdc-119">Attach the file to your support case.</span></span>
