---
title: Grup e-posta Microsoft 365 değiştirme
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930749"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Grup e-posta Microsoft 365 değiştirme

Bir grup yöneticisinin e-posta Microsoft 365 yönetim merkezini kullanarak değiştirebilirsiniz. Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.

Ayrıca, bir kullanıcı grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu Microsoft 365 kullanabilirsiniz:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Örnek: 

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
