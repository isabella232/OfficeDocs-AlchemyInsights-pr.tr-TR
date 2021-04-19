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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b9661-102">Microsoft 365 grubunun e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="b9661-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b9661-103">Yönetim merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b9661-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b9661-104">Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="b9661-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b9661-105">Ayrıca, Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu da kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b9661-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="b9661-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b9661-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b9661-107">Örnek: </span><span class="sxs-lookup"><span data-stu-id="b9661-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
