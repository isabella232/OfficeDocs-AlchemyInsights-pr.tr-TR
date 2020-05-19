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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283264"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="b8f1b-102">Microsoft 365 grubunun e-posta adresini değiştirme</span><span class="sxs-lookup"><span data-stu-id="b8f1b-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="b8f1b-103">Yönetici merkezini kullanarak bir Microsoft 365 grubunun e-posta adresini değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b8f1b-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b8f1b-104">Grubu seçin ve @edit e-posta adresini seçin.</span><span class="sxs-lookup"><span data-stu-id="b8f1b-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b8f1b-105">Bir Microsoft 365 grubunun birincil SMTP adresini değiştirmek için EXO PowerShell komutunu aşağıdaki leri de kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b8f1b-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="b8f1b-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b8f1b-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b8f1b-107">Örnek:</span><span class="sxs-lookup"><span data-stu-id="b8f1b-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
