---
title: SharePoint Designer bağlantı sorunları
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727191"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="70991-102">SharePoint Designer bağlantı sorunları</span><span class="sxs-lookup"><span data-stu-id="70991-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="70991-103">SharePoint Designer 'ın SharePoint sitelerinde bağlantı sorunları yaşıyorsanız, lütfen aşağıdaki ortak çözümleri deneyin.</span><span class="sxs-lookup"><span data-stu-id="70991-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="70991-104">Adım 1: SharePoint Designer 2013 SharePoint Designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ve [SharePoint Designer 2013 için 2 Ağustos 2016 güncelleştirmesi](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)ile güncelleştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="70991-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="70991-105">Adım 2: yerel önbellek dosyalarını temizleyin:</span><span class="sxs-lookup"><span data-stu-id="70991-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="70991-106">SharePoint Designer 2013 'i kapatın.</span><span class="sxs-lookup"><span data-stu-id="70991-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="70991-107">Yerel bilgisayarda, aşağıdaki klasörlerden her birinde bulunan tüm dosyaları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="70991-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="70991-108">%APPDATA%\Microsoft\Web sunucusu Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="70991-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="70991-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="70991-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="70991-110">%USERPROFILE%\appdata\local\microsoft\websitecache</span><span class="sxs-lookup"><span data-stu-id="70991-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="70991-111">SharePoint Designer 2013 açın ve çalışıp çalışmadığını görmek için hesabı yeniden girin.</span><span class="sxs-lookup"><span data-stu-id="70991-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="70991-112">Adım 3: [Windows cihazlarında Office 2013 Için modern kimlik doğrulamasını etkinleştirin](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="70991-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="70991-113">Adım 4: yöneticilerin SharePoint Designer bağlantısına izin vermesi için SharePoint Yönetim Merkezi ayarlarındaki **özel komut dosyasına Izin vermesi** gerekir.</span><span class="sxs-lookup"><span data-stu-id="70991-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="70991-114">Daha fazla [bilgi için bkz](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="70991-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


