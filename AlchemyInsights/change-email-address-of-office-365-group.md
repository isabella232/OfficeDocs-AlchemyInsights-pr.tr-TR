---
title: Microsoft 365 grubunun e-posta adresini değiştirme
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819064"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grubunun e-posta adresini değiştirme

Yönetim merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz. Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.

Ayrıca, Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu da kullanabilirsiniz:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Örnek: 

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
