---
title: SharePoint Designer bağlantı sorunları
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511564"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="a51d9-102">SharePoint Designer bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="a51d9-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="a51d9-103">SharePoint Designer SharePoint sitelerine bağlantı sorunları yaşıyorsa, lütfen aşağıdaki ortak çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="a51d9-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="a51d9-104">Adım 1: SharePoint Designer 2013'ün [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [SharePoint Designer 2013 için 2 Ağustos 2016 Güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)ile güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="a51d9-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="a51d9-105">Adım 2: Yerel önbellek dosyalarını temizleyin:</span><span class="sxs-lookup"><span data-stu-id="a51d9-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="a51d9-106">SharePoint Designer 2013'u kapatın.</span><span class="sxs-lookup"><span data-stu-id="a51d9-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="a51d9-107">Yerel bilgisayarda, aşağıdaki klasörlerin her birinde bulunan tüm dosyaları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="a51d9-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="a51d9-108">%APPDATA%\Microsoft\Web Sunucusu Uzantıları\Önbellek</span><span class="sxs-lookup"><span data-stu-id="a51d9-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="a51d9-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyÖnbellek</span><span class="sxs-lookup"><span data-stu-id="a51d9-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="a51d9-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteÖnbellek</span><span class="sxs-lookup"><span data-stu-id="a51d9-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="a51d9-111">SharePoint Designer 2013'u açın ve çalışıp çalışmadığına görmek için hesabı yeniden girin.</span><span class="sxs-lookup"><span data-stu-id="a51d9-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="a51d9-112">Adım 3: [Windows Aygıtlarında Office 2013 için Modern Kimlik Doğrulamayı Etkinleştirin.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="a51d9-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="a51d9-113">Adım 4: Yöneticilerin SharePoint Designer bağlantısına izin vermek için SharePoint Yönetici Merkezi ayarlarında **Özel Komut Dosyasına İzin** Vermeleri Gerekir.</span><span class="sxs-lookup"><span data-stu-id="a51d9-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="a51d9-114">Bkz. Daha fazla bilgi için [özel komut dosyasına izin ver veya engelleyin.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="a51d9-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


