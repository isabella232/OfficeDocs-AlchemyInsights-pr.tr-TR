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
# <a name="troubleshooting-pst-import-issues"></a>PST içeri aktarma sorunlarını giderme

- Outlook istemcisinin kendisinde içeri aktarıyorsanız, lütfen [Outlook .pst dosyasını içeri aktarma sorunlarını düzeltme](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e) makalesine bakın.

- İçeri Aktarma Hizmetini kullanıyorsanız ve işlem takıldıysa, Azure Depolama konumuna yüklediğiniz her PST dosyasının 20 GB’tan büyük olmaması gerektiğini unutmayın.  20 GB2tan büyük PST dosyaları PST içeri aktarma işleminin performansını etkileyebilir.

- Belirli bir İçeri aktarma işinin durumunu doğrulamak istiyorsanız, [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) komutunu kullanabilirsiniz.

- İçeri aktarma hizmetiyle ilgili tüm ayrıntılar için lütfen [Kuruluşunuzun PST dosyalarını içeri aktarmaya genel bakış](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide) makalesine bakın.
