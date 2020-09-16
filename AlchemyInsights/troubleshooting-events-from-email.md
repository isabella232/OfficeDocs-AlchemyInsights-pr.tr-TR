---
title: E-postadan sorun giderme olayları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658754"
---
# <a name="troubleshooting-events-from-email"></a>E-postadan sorun giderme olayları

1. Özelliğin posta kutusu için etkinleştirildiğini doğrulama: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Ardından ' e-postadaki etkinlikler ' günlüklerine bakın **dışarı aktarma-MailboxDiagnosticLogs <mailbox> -Component timeprofile**

3. ' E-postadaki etkinlikler ' günlüklerinde, posta kutusundaki öğeyle eşleşen ınternetmessageıd öğesini bulun.  

4. TrustScore öğenin eklenip eklenmeyeceğini belirler. Olaylar yalnızca TrustScore = "güvenilen" olarak eklenir.

TrustScore, Ileti üstbilgisindeki SPF, Vseçkim veya DMARC özellikleri tarafından belirlenir.

Bu özellikleri görüntülemek için:

**Masaüstü Outlook**

- Öğeyi açma
- Dosya-> özellikleri-> Internet üstbilgileri

veya

**MFCMapi**

- Gelen kutusu 'nda öğeye gitme
- PR_TRANSPORT_MESSAGE_HEADERS_W arama

Bu özellikler, taşıma ve yönlendirme sırasında belirlenir ve kaydedilir. Daha fazla sorun giderme için, SPF, CıKIM ve. veya DMARC 'daki hatalar hakkında aktarım desteğiyle izlemeniz gerekebilir.