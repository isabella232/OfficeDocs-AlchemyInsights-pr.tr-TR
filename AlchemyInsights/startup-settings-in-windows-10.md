---
title: Windows 10 ' da başlangıç ayarları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751155"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="fccaa-102">Windows 10 ' da başlangıç ayarları</span><span class="sxs-lookup"><span data-stu-id="fccaa-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="fccaa-103">**Başlangıçta otomatik olarak çalıştırılan uygulamaları değiştirme**</span><span class="sxs-lookup"><span data-stu-id="fccaa-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="fccaa-104">[Ayarlar > uygulamalar > başlatma](ms-settings:startupapps?activationSource=GetHelp)'ya gidin.</span><span class="sxs-lookup"><span data-stu-id="fccaa-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="fccaa-105">Başlangıçta çalıştırmak istediğiniz tüm **uygulamaları açık olduğundan emin olun.**</span><span class="sxs-lookup"><span data-stu-id="fccaa-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="fccaa-106">**Başlangıçta otomatik olarak çalışacak bir uygulama ekleme**</span><span class="sxs-lookup"><span data-stu-id="fccaa-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="fccaa-107">**Başlat** 'a tıklayın veya dokunun ve başlangıç sırasında çalıştırmak istediğiniz uygulamayı bulun.</span><span class="sxs-lookup"><span data-stu-id="fccaa-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="fccaa-108">Uygulamayı sağ tıklatın, **diğer**'i ve sonra da **dosya konumunu aç**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="fccaa-109">Uygulama kısayolunun kaydedildiği konum açılır.</span><span class="sxs-lookup"><span data-stu-id="fccaa-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="fccaa-110">Dosya konumu için açık bir seçenek yoksa, uygulama başlangıç sırasında çalıştırılamaz.</span><span class="sxs-lookup"><span data-stu-id="fccaa-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="fccaa-111">Dosya konumu açıkken **Windows logo tuşu + R**tuşlarına basın, **kabuk: başlatma**yazın ve **Tamam**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="fccaa-112">Başlangıç klasörü açılır.</span><span class="sxs-lookup"><span data-stu-id="fccaa-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="fccaa-113">Uygulamanın kısayolunu kopyalayıp dosya konumundan Başlangıç klasörüne yapıştırın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="fccaa-114">**Gelişmiş başlatma seçenekleri (güvenli mod, UEFı ayarları ve başka bir cihazdan önyükleme dahil)**</span><span class="sxs-lookup"><span data-stu-id="fccaa-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="fccaa-115">Bu adımlar bilgisayarınızı yeniden başlatacak olduğundan çalışmanızı kaydedin ve tüm açık belgeleri kapatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="fccaa-116">[& güvenlik > kurtarma > ayarlar](ms-settings:recovery?activationSource=GetHelp)'a gidin.</span><span class="sxs-lookup"><span data-stu-id="fccaa-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="fccaa-117">**Gelişmiş başlatma**'nın altında **Şimdi yeniden Başlat**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="fccaa-118">Bilgisayarınız bir seçenek belirtin ekranı yeniden başlatıldıktan sonra:</span><span class="sxs-lookup"><span data-stu-id="fccaa-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="fccaa-119">USB sürücüsü gibi bir cihazdan önyüklemek için, **cihaz kullan**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="fccaa-120">UEFı ayarları (bazen BIOS kurulumu olarak adlandırılır) girmek için, **Gelişmiş seçenekler > > UEFI üretici yazılımı ayarları**'nı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="fccaa-121">Güvenli Mod girmek veya Gelişmiş başlatma ayarlarını değiştirmek için, **Gelişmiş seçenekler > >** **Restart**</span><span class="sxs-lookup"><span data-stu-id="fccaa-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="fccaa-122">[BitLocker kurtarma anahtarınızı](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)girmeniz istenebilir.</span><span class="sxs-lookup"><span data-stu-id="fccaa-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="fccaa-123">Bilgisayarınız yeniden başlatıldıktan sonra, kullanmak istediğiniz başlangıç ayarını tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fccaa-123">After your PC restarts again, click the startup setting you want to use.</span></span>