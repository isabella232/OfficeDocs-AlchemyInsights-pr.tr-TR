---
title: Sorun Giderme OneDrive performansı
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 5416da63851de8b0b45e1d5c0cef24b03db40e6e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054974"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="52ccf-102">Sorun Giderme OneDrive performansı</span><span class="sxs-lookup"><span data-stu-id="52ccf-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="52ccf-103">OneDrive ile beklenenden daha yavaş bir eşitleme veya benzer performans sorunları yaşıyorsanız:</span><span class="sxs-lookup"><span data-stu-id="52ccf-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="52ccf-104">[Hizmet Durumu Panosu'nu](https://portal.office.com/adminportal/home?ref=/servicehealth)kullanarak bilinen bir sorun olmadığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="52ccf-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="52ccf-105">Tüm dosyalarınızı indirmek ve cihazınızda depolama alanı kullanmak zorunda kalmadan OneDrive'da tüm dosyalarınıza erişebilmeniz için [İsteğe Bağlı Dosyaları etkinleştirin.](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US)</span><span class="sxs-lookup"><span data-stu-id="52ccf-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="52ccf-106">Ağ planlaması ve performansı için [en iyi uygulamaları gözden geçirin.](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)</span><span class="sxs-lookup"><span data-stu-id="52ccf-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="52ccf-107">Özellikle bir aygıtı ilk kez eşitledikten sonra [yükleme ve indirme hızını en üst düzeye çıkarın.](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)</span><span class="sxs-lookup"><span data-stu-id="52ccf-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="52ccf-108">Bir kitaplığı 100.000'den fazla öğeyle eşitlüyorsanız, OneDrive eşitleme uzun süre sıkışmış görünebilir veya durum xMB'nin 0KB Işlemesini gösterir."</span><span class="sxs-lookup"><span data-stu-id="52ccf-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="52ccf-109">[OneDrive'ın desteklenen 300.000 dosya sınırının](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)yanı sıra [100.000'den fazla dosyayı eşitleme hakkında daha fazla bilgi edinin.](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="52ccf-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="52ccf-110">Bir kullanıcı kullanım sınırlarını aştığında, SharePoint Online bu kullanıcı hesabından gelen diğer istekleri kısa bir süre için daraltır.</span><span class="sxs-lookup"><span data-stu-id="52ccf-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="52ccf-111">Gaz etkinken tüm kullanıcı eylemleri daraltılır.</span><span class="sxs-lookup"><span data-stu-id="52ccf-111">All user actions are throttled while the throttle is in effect.</span></span>
