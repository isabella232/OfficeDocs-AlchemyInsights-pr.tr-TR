---
title: E-postadan Sorun Giderme Etkinlikleri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569400"
---
# <a name="troubleshooting-events-from-email"></a>E-postadan Sorun Giderme Etkinlikleri

1. Posta kutusu için özelliğin etkinleştirilen olduğunu doğrulayın: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Sonra 'E-posta dan Olaylar' günlükleri **İhracat-MailboxDiagnosticLogs <mailbox> -Bileşen TimeProfile** bakmak

3. 'E-postadan Olaylar' günlüklerinde, posta kutusundaki öğeyle eşleşen InternetMessageId'i bulun.  

4. TrustScore, öğenin ekilip eklenmediğini belirler. Olaylar yalnızca TrustScore = "Güvenilen" ise eklenir.

Güven Puanı, İleti Üstbilgisinde bulunan SPF, Dkim veya Dmarc özellikleri tarafından belirlenir.

Bu özellikleri görüntülemek için:

**Masaüstü Outlook**

- Öğeyi açma
- Dosya -> Özellikleri -> Internet Başlıkları

veya

**MFCMapi**

- Gelen kutusundaki öğeye gidin
- PR_TRANSPORT_MESSAGE_HEADERS_W arayın

Bu özellikler taşıma ve yönlendirme sırasında belirlenir ve kaydedilir. Daha fazla sorun giderme için, SPF, DKIM ve.veya DMARC'taki hatalar hakkında Transport Support ile izlemeniz gerekebilir.