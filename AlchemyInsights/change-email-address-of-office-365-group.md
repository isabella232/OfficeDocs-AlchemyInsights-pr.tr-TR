---
title: Microsoft 365 grubunun e-posta adresini değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283264"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365 grubunun e-posta adresini değiştirme

Yönetici merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz. Grubu seçin ve @edit e-posta adresini seçin.

Bir Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu aşağıdaki leri de kullanabilirsiniz:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Örnek:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
