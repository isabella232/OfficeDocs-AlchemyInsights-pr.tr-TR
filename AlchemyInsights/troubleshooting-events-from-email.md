---
title: E-postadan Etkinliklerle ilgili sorunları giderme
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834859"
---
# <a name="troubleshooting-events-from-email"></a>E-postadan Etkinliklerle ilgili sorunları giderme

1. Posta kutusu için özelliğin etkinleştirildiğinden emin olun: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Ardından "E-postadan Etkinlikler" günlüklerine **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. 'E-postadan Etkinlikler' günlüklerinde, posta kutusunda öğeyle eşleşen InternetMessageId'i bulun.  

4. TrustScore, öğenin ekli olup olmadığını belirler. Olaylar yalnızca TrustScore = "Trusted" ise eklenir.

TrustScore, İleti Üst Bilgisinde bulunan SPF, Dkim veya Dmarc özellikleri tarafından belirlenir.

Bu özellikleri görüntülemek için:

**Masaüstü Outlook**

- Öğeyi açma
- File -> Properties -> Internet Headers

veya

**MFCMapi**

- Gelen kutusunda öğeye gider
- Daha fazla PR_TRANSPORT_MESSAGE_HEADERS_W

Bu özellikler aktarım ve yönlendirme sırasında belirlenir ve kaydedilir. Sorun gidermeye yönelik daha fazla sorun gidermek için SPF, DKIM ve.veya DMARC'daki başarısızlıklar hakkında Aktarım Desteği'ne ihtiyacınız olabilir.