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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187741"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="0a958-102">Teams kilitlenmesi</span><span class="sxs-lookup"><span data-stu-id="0a958-102">Teams client crashing</span></span>

<span data-ttu-id="0a958-103">Teams istemciniz kilitleniyorsa şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="0a958-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0a958-104">Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0a958-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0a958-105">Tüm url'lerin [Microsoft 365 erişilebilir olduğundan](/microsoftteams/connectivity-issues) emin olun.</span><span class="sxs-lookup"><span data-stu-id="0a958-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0a958-106">Kiracı yönetici hesabınızla oturum açın ve kesinti [veya](/office365/enterprise/view-service-health) hizmet performansında bir düşüş olmadığını doğrulamak için Hizmet Durumu Pano'nıza göz atabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0a958-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="0a958-107">Teams Uygulamasını kaldırıp yeniden yükleyin</span><span class="sxs-lookup"><span data-stu-id="0a958-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="0a958-108">Bilgisayarınızda %appdata%\Microsoft\Teams\ klasörüne gidin ve o dizindeki tüm dosyaları silin.</span><span class="sxs-lookup"><span data-stu-id="0a958-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="0a958-109">[Teams Uygulamasını indirip](https://www.microsoft.com/microsoft-teams/download-app)yükleyin ve mümkünse yönetici olarak Teams yükleyin (Teams yükleyicisini sağ tıklatın ve varsa Yönetici olarak **çalıştır'ı** seçin).</span><span class="sxs-lookup"><span data-stu-id="0a958-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="0a958-110">Teams istemciniz hala kilitlenmeye devam ediyorsa, sorunu yeniden oluşturmaya deneyin.</span><span class="sxs-lookup"><span data-stu-id="0a958-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="0a958-111">Şunları biliyorsanız:</span><span class="sxs-lookup"><span data-stu-id="0a958-111">If you can:</span></span>

1. <span data-ttu-id="0a958-112">Adımlarınızı yakalamak için Adım Kaydedicisi'yi kullanın.</span><span class="sxs-lookup"><span data-stu-id="0a958-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="0a958-113">TÜM gereksiz veya gizli uygulamaları kapatın.</span><span class="sxs-lookup"><span data-stu-id="0a958-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="0a958-114">Etkilenen kullanıcı hesabıyla oturum açmış durumdayken Adım Kaydedicisi'ni başlatarak sorunu yeniden üretin.</span><span class="sxs-lookup"><span data-stu-id="0a958-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="0a958-115">[Kaydedilen yeniden proje adımlarını yakalayan ekip günlüklerini toplayın.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="0a958-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="0a958-116">**Not:** Etki alanı etki olan kullanıcının oturum açma adresini yakalamayı unutmayın.</span><span class="sxs-lookup"><span data-stu-id="0a958-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="0a958-117">Dökümü ve/veya Hata demeti bilgilerini toplayın (Windows).</span><span class="sxs-lookup"><span data-stu-id="0a958-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="0a958-118">Kilitlenme Windows makinede Powershell'i çalıştırın ve aşağıdaki komutları çalıştırın (her komuttan sonra Enter tuşuna basın):</span><span class="sxs-lookup"><span data-stu-id="0a958-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="0a958-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="0a958-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="0a958-120">Metin dosyası oluşturularak ekran üzerinde görüntülendiğinde, dosyayı kaydedin ve hizmet isteğine iliştirin.</span><span class="sxs-lookup"><span data-stu-id="0a958-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
