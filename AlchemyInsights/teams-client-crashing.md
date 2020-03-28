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
# <a name="teams-client-crashing"></a><span data-ttu-id="40446-102">Teams istemcisi kilitleniyor mu?</span><span class="sxs-lookup"><span data-stu-id="40446-102">Teams client crashing?</span></span>

<span data-ttu-id="40446-103">Teams istemciniz kilitleniyorsa şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="40446-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="40446-104">Teams masaüstü uygulamasını kullanıyorsanız [uygulamanın tamamen güncel olduğundan emin olun](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="40446-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="40446-105">Tüm [Office 365 URL’lerinin ve adres aralıklarının](https://docs.microsoft.com/microsoftteams/connectivity-issues) erişilebilir durumda olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="40446-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="40446-106">Kesinti veya hizmet performansında düşüş olmadığından emin olmak için yönetici hesabınızla oturum açın ve [Hizmet Durumu Panonuzu](https://docs.microsoft.com/office365/enterprise/view-service-health) denetleyin.</span><span class="sxs-lookup"><span data-stu-id="40446-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="40446-107">Son olarak, Teams istemci önbelleğinizi temizlemeyi deneyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="40446-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="40446-108">Microsoft Teams masaüstü istemcisinden tamamen çıkın.</span><span class="sxs-lookup"><span data-stu-id="40446-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="40446-109">Simge Tepsisinden **Teams**’e sağ tıklayıp **Çık**’a tıklayabilir veya Görev Yöneticisi’ni çalıştırıp işlemi tamamen sonlandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="40446-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="40446-110">Dosya Gezgini’ne gidin ve %appdata%\Microsoft\teams yazın.</span><span class="sxs-lookup"><span data-stu-id="40446-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="40446-111">Dizine girdiğinizde şu klasörlerden birkaç tanesini görürsünüz:</span><span class="sxs-lookup"><span data-stu-id="40446-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="40446-112">**Uygulama Önbelleği** içinden Önbellek’e gidip Önbellek konumundaki (%appdata%\Microsoft\teams\application cache\cache) dosyalardan dilediğinizi silin.</span><span class="sxs-lookup"><span data-stu-id="40446-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="40446-113">**Blob_storage** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="40446-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="40446-114">**Önbellek** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="40446-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="40446-115">**Veritabanları** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="40446-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="40446-116">**GPUCache** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="40446-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="40446-117">**IndexedDB** içindeki .db uzantılı dosyayı silin: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="40446-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="40446-118">**Yerel Depolama** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="40446-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="40446-119">Son olarak, **tmp** içindeki tüm dosyaları silin: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="40446-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="40446-120">Teams istemcinizi yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="40446-120">Restart your Teams client.</span></span>
