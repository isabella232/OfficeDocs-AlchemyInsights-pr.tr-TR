---
title: Çevrimiçi SharePoint izin düzeylerini
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760712"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="82b37-102">SharePoint Designer bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="82b37-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="82b37-103">Lütfen SharePoint Designer SharePoint sitelerine bağlantı sorunlar yaşanıyorsa aşağıdaki ortak çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="82b37-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="82b37-104">Adım 1: Doğrulama SharePoint Designer güncelleştirilir.</span><span class="sxs-lookup"><span data-stu-id="82b37-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="82b37-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="82b37-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="82b37-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="82b37-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="82b37-107">SharePoint Designer 2013 (KB3114721) güncelleştirmesi</span><span class="sxs-lookup"><span data-stu-id="82b37-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="82b37-108">Adım 2: yerel önbellek dosyaları Temizle</span><span class="sxs-lookup"><span data-stu-id="82b37-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="82b37-109">SharePoint Designer 2013 kapatın.</span><span class="sxs-lookup"><span data-stu-id="82b37-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="82b37-110">Yerel bilgisayarda önbelleğe alınmış dosyaları silmek için aşağıdaki klasörleri bulun.</span><span class="sxs-lookup"><span data-stu-id="82b37-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="82b37-111">Başlat, Çalıştır ve her biri altında bulunan tüm dosyaları sil konumları aşağıda.</span><span class="sxs-lookup"><span data-stu-id="82b37-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="82b37-112">%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="82b37-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="82b37-113">SharePoint Designer 2013 açın ve yeniden çalışıp çalışmadığını görmek için bir hesap girin.</span><span class="sxs-lookup"><span data-stu-id="82b37-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="82b37-114">Adım 3: [Modern Office 2013 aygıtlarda Windows kimlik doğrulamasını etkinleştirmek](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="82b37-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="82b37-115">Adım 4: Yöneticiler SharePoint Designer bağlantıya izin veren özel komut dosyasına izin gerekir.</span><span class="sxs-lookup"><span data-stu-id="82b37-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="82b37-116">Ayrıntılı adımlar, örnekler ve dikkat edilmesi gereken noktalar için bkz: [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="82b37-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


