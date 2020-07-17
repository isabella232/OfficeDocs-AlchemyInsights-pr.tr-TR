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
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="07742-102">Sorun Giderme OneDrive çöküyor</span><span class="sxs-lookup"><span data-stu-id="07742-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="07742-103">OneDrive sürekli olarak çöküyorsa, şu sorun giderme adımlarını deneyin:</span><span class="sxs-lookup"><span data-stu-id="07742-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="07742-104">**Kayıt defteri anahtarlarının ayarlı olmadığından emin olun:**</span><span class="sxs-lookup"><span data-stu-id="07742-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="07742-105">Kayıt Defteri Düzenleyicisi'ni kullanarak HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive'a gidin</span><span class="sxs-lookup"><span data-stu-id="07742-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="07742-106">DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak değiştirin.</span><span class="sxs-lookup"><span data-stu-id="07742-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="07742-107">Start'a giderek OneDrive'ı el ile başlatın</span><span class="sxs-lookup"><span data-stu-id="07742-107">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="07742-109">, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="07742-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="07742-110">**OneDrive'ı Sıfırla:**</span><span class="sxs-lookup"><span data-stu-id="07742-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="07742-111">Notlar:</span><span class="sxs-lookup"><span data-stu-id="07742-111">Notes:</span></span>

- <span data-ttu-id="07742-112">OneDrive'ı sıfırlamak, mevcut eşitleme bağlantılarınızın bağlantısını keser (ayarlanmışsa kişisel OneDrive'ınız dahil).</span><span class="sxs-lookup"><span data-stu-id="07742-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="07742-113">OneDrive'ı bilgisayarınızda sıfırlayarak dosya veya veri kaybetmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="07742-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="07742-114">**OneDrive'ı sıfırlamak için:**</span><span class="sxs-lookup"><span data-stu-id="07742-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="07742-115">Windows tuşu ve R tuşuna basarak Çalıştır iletişim kutusunu açın.</span><span class="sxs-lookup"><span data-stu-id="07742-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="07742-116">%localappdata%\Microsoft\OneDrive\onedrive.exe /reset yazın ve Tamam tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="07742-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="07742-117">Komut penceresi kısa bir süre görünebilir.</span><span class="sxs-lookup"><span data-stu-id="07742-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="07742-118">Start'a giderek OneDrive'ı el ile başlatın</span><span class="sxs-lookup"><span data-stu-id="07742-118">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="07742-120">, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="07742-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="07742-121">Notlar:</span><span class="sxs-lookup"><span data-stu-id="07742-121">Notes:</span></span>

- <span data-ttu-id="07742-122">Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiyseniz, eşitleme tamamlandıktan sonra bunu tekrar yapmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="07742-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="07742-123">Daha fazla bilgi için [bilgisayarınızla eşitlenebilmek için hangi OneDrive klasörlerini](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   seç'i okuyun.</span><span class="sxs-lookup"><span data-stu-id="07742-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="07742-124">Kişisel OneDrive ve OneDrive for Business için bunu tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="07742-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>