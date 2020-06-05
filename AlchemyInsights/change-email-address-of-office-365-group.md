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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580677"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grubunun e-posta adresini değiştirme

Yönetici merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz. Grubu seçin ve @edit e-posta adresini seçin.

Bir Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu aşağıdaki leri de kullanabilirsiniz:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Örnek:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
