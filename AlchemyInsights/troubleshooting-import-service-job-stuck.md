---
title: İçeri Aktarma Hizmeti işi takılmış sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125497"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="4c3db-102">İçeri Aktarma Hizmeti işi takılmış sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="4c3db-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="4c3db-103">Hizmet işlerini içeri aktarmanın takılmış veya başarısız olduğu sorunlar yaşıyorsanız, şunları incele ve deneyin:</span><span class="sxs-lookup"><span data-stu-id="4c3db-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="4c3db-104">PST dosyasının boyutunu gözden geçirme.</span><span class="sxs-lookup"><span data-stu-id="4c3db-104">Review the size of of the PST file.</span></span> <span data-ttu-id="4c3db-105">İçeri aktarma için bir PST dosyasının en çok önerilen boyutu 20 GB'dır.</span><span class="sxs-lookup"><span data-stu-id="4c3db-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="4c3db-106">Bozulma nedeniyle öğeleri atlamadan şüpheleniyorsanız PST dosyalarında Scanpst.exe tanılamak ve düzeltmek için bu dosyaları çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="4c3db-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="4c3db-107">İçeri aktarma sırasında "MapiExceptionShutoffQuotaExceeded" hatasını görüyorsanız, hedef posta kutusunun istenen PST dosyalarını içeri aktarma kapasitesine sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="4c3db-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="4c3db-108">PST içeri aktarma iş sorunlarını giderme hakkında daha fazla bilgi için [bkz. PST içeri aktarma işleriyle ilgili sorunları giderme.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="4c3db-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="4c3db-109">PST'leri Outlook'a içeri aktarma sorunlarını çözme hakkında bilgi için bkz. Outlook .pst dosyasını [(microsoft.com) içeri aktarma sorunlarını düzeltme.](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="4c3db-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>