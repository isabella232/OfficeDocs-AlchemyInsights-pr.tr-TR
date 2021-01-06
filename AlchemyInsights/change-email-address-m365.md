---
title: Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme
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
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756577"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme

[Microsoft 365 yönetim merkezi](https://admin.microsoft.com/)’ni kullanarak bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirebilirsiniz. Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.

Ayrıca bir Microsoft 365 grubunun/Teams ekibinin birincil SMTP adresini değiştirmek için aşağıdaki EXO PowerShell komutunu kullanabilirsiniz:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Örnek: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
