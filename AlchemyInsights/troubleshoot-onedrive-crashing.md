---
title: OneDrive kilitlenme sorunlarını giderme
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826219"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="d2821-102">OneDrive kilitlenme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="d2821-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="d2821-103">OneDrive art arda kilitlenirse şu sorun giderme adımlarını deneyin:</span><span class="sxs-lookup"><span data-stu-id="d2821-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="d2821-104">**Kayıt defteri anahtarlarının ayarlanmay olduğundan emin olun:**</span><span class="sxs-lookup"><span data-stu-id="d2821-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="d2821-105">Kayıt Defteri Düzenleyicisi'ni kullanarak Kayıt Defteri'HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="d2821-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="d2821-106">DisableFileSyncNGSC varsa ve 1 olarak ayarlanmışsa, anahtarı açın ve değeri 0 olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="d2821-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="d2821-107">Başlat'a gidip OneDrive'ı el ile başlatma</span><span class="sxs-lookup"><span data-stu-id="d2821-107">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d2821-109">yazın, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d2821-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d2821-110">**OneDrive'ı sıfırlama:**</span><span class="sxs-lookup"><span data-stu-id="d2821-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="d2821-111">Notlar:</span><span class="sxs-lookup"><span data-stu-id="d2821-111">Notes:</span></span>

- <span data-ttu-id="d2821-112">OneDrive'ı sıfırlayarak mevcut tüm eşitleme bağlantılarınızı (ayarlanmışsa kişisel OneDrive dahil) bağlantısını kesebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d2821-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="d2821-113">Bilgisayarınızda OneDrive'ı sıfırlayarak dosyalarınız veya verileriniz kaybetmezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d2821-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="d2821-114">**OneDrive'ı sıfırlamak için:**</span><span class="sxs-lookup"><span data-stu-id="d2821-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="d2821-115">Windows tuşu ve R tuşuna basarak Çalıştır iletişim kutusunu açın.</span><span class="sxs-lookup"><span data-stu-id="d2821-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="d2821-116">%localappdata%\Microsoft\OneDrive\onedrive.exe /reset yazın ve Tamam'a basın.</span><span class="sxs-lookup"><span data-stu-id="d2821-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="d2821-117">Kısa süreli olarak bir Komut penceresi görünebilir.</span><span class="sxs-lookup"><span data-stu-id="d2821-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="d2821-118">Başlat'a gidip OneDrive'ı el ile başlatma</span><span class="sxs-lookup"><span data-stu-id="d2821-118">Manually launch OneDrive by going to Start</span></span> ![Windows tuşuna basın](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="d2821-120">yazın, arama kutusuna OneDrive yazın ve ardından OneDrive masaüstü uygulamasına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="d2821-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="d2821-121">Notlar:</span><span class="sxs-lookup"><span data-stu-id="d2821-121">Notes:</span></span>

- <span data-ttu-id="d2821-122">Sıfırlamadan önce yalnızca bazı klasörleri eşitlemeyi seçtiysanız, eşitleme tamamlandıktan sonra bunu yeniden eşitlemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="d2821-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="d2821-123">Daha [fazla bilgi için Hangi OneDrive klasörlerinin bilgisayarınıza eşitleneceklerini](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)seçme   makalesi'ni okuyun.</span><span class="sxs-lookup"><span data-stu-id="d2821-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="d2821-124">Bunu kişisel OneDrive ve OneDrive İş için tamamlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="d2821-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>