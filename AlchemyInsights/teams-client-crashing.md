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
# <a name="teams-client-crashing"></a><span data-ttu-id="902fc-102">Teams istemcisi kilitleniyor mu?</span><span class="sxs-lookup"><span data-stu-id="902fc-102">Teams client crashing?</span></span>

<span data-ttu-id="902fc-103">Teams istemciniz kilitleniyorsa şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="902fc-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="902fc-104">Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="902fc-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="902fc-105">Tüm Microsoft [365 URL'leri ve adres aralıklarını erişilebilir olduğundan](https://docs.microsoft.com/microsoftteams/connectivity-issues) emin olun.</span><span class="sxs-lookup"><span data-stu-id="902fc-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="902fc-106">Kiracı yönetici hesabınızla oturum açın ve kesinti [veya](https://docs.microsoft.com/office365/enterprise/view-service-health) hizmet performansında bir düşüş olmadığını doğrulamak için Hizmet Durumu Pano'nıza göz atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="902fc-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="902fc-107">Teams Uygulamasını kaldırma ve yeniden yükleme (bağlantı)</span><span class="sxs-lookup"><span data-stu-id="902fc-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="902fc-108">Bilgisayarınızda %appdata%\Microsoft\teams\ klasörüne gidin ve bu dizindeki tüm dosyaları silin.</span><span class="sxs-lookup"><span data-stu-id="902fc-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="902fc-109">[Teams Uygulamasını indirip yükleyin ve](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)mümkünse Teams'i yönetici olarak yükleyin (Teams yükleyicisi'ne sağ tıklayın ve varsa "Yönetici olarak çalıştır"ı seçin).</span><span class="sxs-lookup"><span data-stu-id="902fc-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="902fc-110">Teams istemciniz hala kilitlenmeye devam ediyorsa sorunu yeniden ürete misiniz?</span><span class="sxs-lookup"><span data-stu-id="902fc-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="902fc-111">Öyleyse:</span><span class="sxs-lookup"><span data-stu-id="902fc-111">If so:</span></span>

1. <span data-ttu-id="902fc-112">Adımlarınızı yakalamak için Adım Kaydedicisi'yi kullanın.</span><span class="sxs-lookup"><span data-stu-id="902fc-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="902fc-113">TÜM gereksiz veya gizli uygulamaları kapatın.</span><span class="sxs-lookup"><span data-stu-id="902fc-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="902fc-114">Etkilenen kullanıcı hesabıyla oturum açmış durumdayken Adım Kaydedicisi'ni başlatarak sorunu yeniden üretin.</span><span class="sxs-lookup"><span data-stu-id="902fc-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="902fc-115">[Kaydedilen yeniden proje adımlarını yakalayan ekip günlüklerini toplayın.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="902fc-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="902fc-116">**Not:** Etki alanı etki olan kullanıcının oturum açma adresini yakalamayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="902fc-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="902fc-117">Dökümü ve/veya Hata demeti bilgilerini (Windows) toplayın.</span><span class="sxs-lookup"><span data-stu-id="902fc-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="902fc-118">Kilitlenmenin olduğu makinede Windows Powershell'i çalıştırın ve aşağıdaki komutları çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="902fc-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="902fc-119">Dosyayı destek olaynıza iliştirin.</span><span class="sxs-lookup"><span data-stu-id="902fc-119">Attach the file to your support case.</span></span>
