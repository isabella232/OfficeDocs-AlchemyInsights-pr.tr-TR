---
title: PST içeri aktarma sorunlarını giderme
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
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826183"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="f44b3-102">PST içeri aktarma sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="f44b3-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="f44b3-103">Outlook istemcisinin kendisinde içeri aktarıyorsanız, lütfen [Outlook .pst dosyasını içeri aktarma sorunlarını düzeltme](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e) makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="f44b3-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="f44b3-104">İçeri Aktarma Hizmetini kullanıyorsanız ve işlem takıldıysa, Azure Depolama konumuna yüklediğiniz her PST dosyasının 20 GB’tan büyük olmaması gerektiğini unutmayın. </span><span class="sxs-lookup"><span data-stu-id="f44b3-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="f44b3-105">20 GB2tan büyük PST dosyaları PST içeri aktarma işleminin performansını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="f44b3-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="f44b3-106">Belirli bir İçeri aktarma işinin durumunu doğrulamak istiyorsanız, [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) komutunu kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f44b3-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="f44b3-107">İçeri aktarma hizmetiyle ilgili tüm ayrıntılar için lütfen [Kuruluşunuzun PST dosyalarını içeri aktarmaya genel bakış](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide) makalesine bakın.</span><span class="sxs-lookup"><span data-stu-id="f44b3-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
