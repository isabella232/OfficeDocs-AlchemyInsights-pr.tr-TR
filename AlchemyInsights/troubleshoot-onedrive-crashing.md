---
title: OneDrive kilitleniyor sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665018"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="d3e12-102">OneDrive kilitleniyor sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="d3e12-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="d3e12-103">OneDrive sürekli kilitleniyor, şu sorun giderme adımlarını deneyin:</span><span class="sxs-lookup"><span data-stu-id="d3e12-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="d3e12-104">**Kayıt defteri anahtarlarının ayarlanmadığından emin olun:**</span><span class="sxs-lookup"><span data-stu-id="d3e12-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="d3e12-105">Kayıt Defteri Düzenleyicisi 'ni kullanarak HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="d3e12-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="d3e12-106">DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak değiştirin.</span><span class="sxs-lookup"><span data-stu-id="d3e12-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="d3e12-107">Başlat 'a giderek OneDrive 'ı el ile başlatın</span><span class="sxs-lookup"><span data-stu-id="d3e12-107">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d3e12-109">, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d3e12-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d3e12-110">**OneDrive 'ı sıfırlayın:**</span><span class="sxs-lookup"><span data-stu-id="d3e12-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="d3e12-111">Notlarında</span><span class="sxs-lookup"><span data-stu-id="d3e12-111">Notes:</span></span>

- <span data-ttu-id="d3e12-112">OneDrive 'ı sıfırlamak, var olan tüm eşitleme bağlantılarınızı (ayarlanmış olan kişisel OneDrive 'ı dahil) bağlantıyı keser.</span><span class="sxs-lookup"><span data-stu-id="d3e12-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="d3e12-113">Bilgisayarınızda OneDrive 'ı sıfırlayarak dosyaları veya verileri kaybetmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d3e12-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="d3e12-114">**OneDrive 'ı sıfırlamak için:**</span><span class="sxs-lookup"><span data-stu-id="d3e12-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="d3e12-115">Windows tuşuna ve R tuşuna basarak bir Run iletişim kutusunu açın.</span><span class="sxs-lookup"><span data-stu-id="d3e12-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="d3e12-116">% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset yazın ve Tamam 'a basın.</span><span class="sxs-lookup"><span data-stu-id="d3e12-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="d3e12-117">Kısaca bir komut penceresi görüntülenebilir.</span><span class="sxs-lookup"><span data-stu-id="d3e12-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="d3e12-118">Başlat 'a giderek OneDrive 'ı el ile başlatın</span><span class="sxs-lookup"><span data-stu-id="d3e12-118">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d3e12-120">, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d3e12-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d3e12-121">Notlarında</span><span class="sxs-lookup"><span data-stu-id="d3e12-121">Notes:</span></span>

- <span data-ttu-id="d3e12-122">Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiyseniz, eşitleme tamamlandığında bunu yeniden yapmalısınız.</span><span class="sxs-lookup"><span data-stu-id="d3e12-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="d3e12-123">Daha fazla bilgi için [hangi OneDrive klasörlerinin bilgisayarınıza eşitleneceğini seçin](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="d3e12-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="d3e12-124">Kişisel OneDrive ve OneDrive Iş için bunu tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d3e12-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>