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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105372"
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