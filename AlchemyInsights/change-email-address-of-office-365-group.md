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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="0d839-102">Microsoft 365 grubunun e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="0d839-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="0d839-103">Yönetici merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0d839-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="0d839-104">Grubu seçin ve @edit e-posta adresini seçin.</span><span class="sxs-lookup"><span data-stu-id="0d839-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="0d839-105">Bir Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu aşağıdaki leri de kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="0d839-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="0d839-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="0d839-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="0d839-107">Örnek:</span><span class="sxs-lookup"><span data-stu-id="0d839-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
