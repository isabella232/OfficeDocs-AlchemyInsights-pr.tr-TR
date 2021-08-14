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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972439"
---
# <a name="troubleshooting-pst-import-issues"></a>PST içeri aktarma sorunlarını giderme

- Bir .pst dosyasının içinde içeri Outlook, [bkz. Outlook .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)dosyasını içeri aktarma sorunlarını düzeltme.

- İçeri Aktarma Hizmeti kullanıyorsanız ve takılmış durumda olursa, Azure depolama alanına yüklediğiniz her PST dosyasının 20 GB'tan büyük Depolama olmadığını unutmayın. 20 GB'tan büyük PST dosyaları PST içeri aktarma işleminin performansını etkileyebilir. Takılmış işlerde sorun giderme hakkında daha fazla [bilgi için bkz. PST içeri aktarma işlerini etkileyen sorunlar](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Belirli bir İçeri Aktarma işinin durumunu doğrulamak için [Get-MailboxImportRequest -batchname kullanın.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- İçeri aktarma hizmeti hakkında tüm ayrıntılar için bkz. [Kuruluş PST dosyalarını içeri aktarmaya genel bakış.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
