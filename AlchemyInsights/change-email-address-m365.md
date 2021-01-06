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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="eaaa8-102">Bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="eaaa8-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="eaaa8-103">[Microsoft 365 yönetim merkezi](https://admin.microsoft.com/)’ni kullanarak bir Microsoft 365 grubunun veya Microsoft Teams ekibinin e-posta adresini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="eaaa8-104">Grubu seçmeniz ve @e-posta adresini düzenle seçeneğini belirlemeniz yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="eaaa8-105">Ayrıca bir Microsoft 365 grubunun/Teams ekibinin birincil SMTP adresini değiştirmek için aşağıdaki EXO PowerShell komutunu kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="eaaa8-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="eaaa8-106">Örnek: </span><span class="sxs-lookup"><span data-stu-id="eaaa8-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
