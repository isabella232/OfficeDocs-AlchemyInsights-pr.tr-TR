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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819100"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme

[Microsoft 365 yönetim merkezi](https://admin.microsoft.com/)’ni kullanarak bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirebilirsiniz. Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.

Ayrıca bir Microsoft 365 grubunun/Teams ekibinin birincil SMTP adresini değiştirmek için aşağıdaki EXO PowerShell komutunu kullanabilirsiniz:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Örnek: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
