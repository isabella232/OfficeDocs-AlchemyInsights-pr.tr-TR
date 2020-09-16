---
title: OneDrive performansına sorun giderme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757905"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="15b3c-102">OneDrive performansına sorun giderme</span><span class="sxs-lookup"><span data-stu-id="15b3c-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="15b3c-103">OneDrive ile beklenenden daha yavaş bir eşitleme veya benzer performans sorunları yaşıyorsanız:</span><span class="sxs-lookup"><span data-stu-id="15b3c-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="15b3c-104">[Hizmet durumu panosunu](https://portal.office.com/adminportal/home?ref=/servicehealth)kullanarak bilinen bir sorun olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="15b3c-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="15b3c-105">OneDrive 'daki tüm dosyalarınıza indirmek ve cihazınızda depolama alanı kullanmak zorunda kalmadan dosyalarınıza erişebilmek için [dosyaları isteğe](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) bağlı olarak etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="15b3c-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="15b3c-106">Ağ planlaması ve performans için [en iyi yöntemleri gözden geçirin](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) .</span><span class="sxs-lookup"><span data-stu-id="15b3c-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="15b3c-107">Bir cihazı ilk kez eşitlemekte, [yükleme ve indirme hızını en yükseğe çıkarın](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43).</span><span class="sxs-lookup"><span data-stu-id="15b3c-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="15b3c-108">100.000 ' den fazla öğe içeren bir kitaplığı eşitleyorsanız, OneDrive eşitlemesi uzun süredir kalmış görünebilir veya durum</span><span class="sxs-lookup"><span data-stu-id="15b3c-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="15b3c-109">100.000 dosyalarını [ve OneDrive 'ın desteklenen 300.000 dosyalarının](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)yanı sıra, daha [fazla bilgi edinin](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) .</span><span class="sxs-lookup"><span data-stu-id="15b3c-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="15b3c-110">Bir Kullanıcı kullanım sınırlarını aştığında, SharePoint Online, kısa bir süre için bu kullanıcı hesabından gelen tüm istekleri kısıtlar.</span><span class="sxs-lookup"><span data-stu-id="15b3c-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="15b3c-111">Azaltma işlemi sürerken tüm Kullanıcı eylemleri daraltıldı.</span><span class="sxs-lookup"><span data-stu-id="15b3c-111">All user actions are throttled while the throttle is in effect.</span></span>
