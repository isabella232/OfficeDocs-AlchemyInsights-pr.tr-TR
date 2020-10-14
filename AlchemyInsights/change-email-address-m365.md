---
title: Microsoft 365 grubunun e-posta adresini değiştirme
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462060"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b67a4-102">Microsoft 365 grubunun e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="b67a4-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b67a4-103">Microsoft 365 grubunun e-posta adresini yönetim merkezini kullanarak değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b67a4-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b67a4-104">Yalnızca grubu seçin ve @edit e-posta adresi 'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="b67a4-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b67a4-105">Ayrıca, bir Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu da kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b67a4-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="b67a4-106">Örnekteki</span><span class="sxs-lookup"><span data-stu-id="b67a4-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
