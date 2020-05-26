---
title: Paylaşım bağlantılarında indirmeyi engelleyin
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358510"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="756e9-102">Paylaşım bağlantılarında indirmeyi engelleyin</span><span class="sxs-lookup"><span data-stu-id="756e9-102">Block download on sharing links</span></span>

<span data-ttu-id="756e9-103">**Engelleme indirme,** Office belgelerine **yalnızca görüntüleme bağlantıları** için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="756e9-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="756e9-104">Bu seçeneği seçtiğinizde, oluşturduğunuz bağlantı üzerinden dosyaya erişen kişiler dosyayı indirme, yazdırma veya kopyalama seçeneklerini görmez.</span><span class="sxs-lookup"><span data-stu-id="756e9-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="756e9-105">Yöneticiler, `BlockDownloadLinksFileType` [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) veya [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets'teki ayarı değiştirerek "engelleme indirme" ayarının yalnızca Office dosyaları için görünüp görünmediğini denetleyebilir.</span><span class="sxs-lookup"><span data-stu-id="756e9-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
