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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="7a014-102">Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="7a014-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="7a014-103">[Microsoft 365 yönetim merkezi](https://admin.microsoft.com/)’ni kullanarak bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7a014-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="7a014-104">Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="7a014-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="7a014-105">Ayrıca bir Microsoft 365 grubunun/Teams ekibinin birincil SMTP adresini değiştirmek için aşağıdaki EXO PowerShell komutunu kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7a014-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="7a014-106">Örnek: </span><span class="sxs-lookup"><span data-stu-id="7a014-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
