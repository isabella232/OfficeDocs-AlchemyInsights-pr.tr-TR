---
title: Eşitlenmiş Kullanıcı Yönetme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823987"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="b24b0-102">Birincil e-posta adresi ayar, kullanıcı özniteliklerini değiştiremiyor veya eşitlenmiş bir kullanıcı kaldır/silemiyor</span><span class="sxs-lookup"><span data-stu-id="b24b0-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="b24b0-103">Ortamınız için dizin eşitlemesi etkinleştirildiyse, bazı kullanıcı veya nesne öznitelikleri Microsoft 365 yönetim merkezi kullanılarak değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="b24b0-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="b24b0-104">Eşitlenmiş kullanıcıları ve onların tüm özniteliklerini tam olarak yönetmek için, yerel Active Directory kullanıcılarınızı ve grup yönetim konsolunuzu (adsiedit.msc) kullanın.</span><span class="sxs-lookup"><span data-stu-id="b24b0-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="b24b0-105">Alternatif olarak, şu yaygın örneklerde gösterildiği gibi Powershell kullanarak eşitlenmiş kullanıcıların tek tek kullanıcılarını veya özniteliklerini değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b24b0-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
