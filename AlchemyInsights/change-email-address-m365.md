---
title: Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995642"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme

[Microsoft 365 yönetim merkezi](https://admin.microsoft.com/)’ni kullanarak bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirebilirsiniz. Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.

Ayrıca bir Microsoft 365 grubunun/Teams ekibinin birincil SMTP adresini değiştirmek için aşağıdaki EXO PowerShell komutunu kullanabilirsiniz:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Örnek: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
