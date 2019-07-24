---
title: SharePoint Designer bağlantı sorunları
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840571"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="8dea7-102">SharePoint Designer bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="8dea7-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="8dea7-103">SharePoint Designer SharePoint sitelerine bağlantı sorunları yaşıyor, lütfen aşağıdaki ortak çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="8dea7-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="8dea7-104">1. adım: SharePoint Designer 2013 [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [2 Ağustos 2016 için SharePoint Designer 2013 güncelleştirme](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)güncelleştirilmiş olduğunu doğrulamak.</span><span class="sxs-lookup"><span data-stu-id="8dea7-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="8dea7-105">Adım 2: yerel önbellek dosyaları temizleyin:</span><span class="sxs-lookup"><span data-stu-id="8dea7-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="8dea7-106">SharePoint Designer 2013 kapatın.</span><span class="sxs-lookup"><span data-stu-id="8dea7-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="8dea7-107">Yerel bilgisayarda, her biri aşağıdaki klasörler içinde bulunan tüm dosyaları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="8dea7-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="8dea7-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="8dea7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="8dea7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="8dea7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="8dea7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="8dea7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="8dea7-111">SharePoint Designer 2013 açın ve yeniden çalışıp çalışmadığını görmek için bir hesap girin.</span><span class="sxs-lookup"><span data-stu-id="8dea7-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="8dea7-112">Adım 3: [Windows cihazlarda Office 2013 için Modern kimlik doğrulamasını etkinleştirin](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8dea7-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="8dea7-113">Adım 4: Yöneticiler **Özel komut dosyası izin vermek** için SharePoint Yönetim Merkezi ayarlarını SharePoint Designer bağlantıya izin vermek için gerekir.</span><span class="sxs-lookup"><span data-stu-id="8dea7-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="8dea7-114">Bkz: [izin ver veya özel komut dosyası engelleme](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) daha fazla bilgi için.</span><span class="sxs-lookup"><span data-stu-id="8dea7-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


