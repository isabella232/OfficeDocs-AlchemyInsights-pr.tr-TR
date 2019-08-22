---
title: Eşzamanlı kullanıcı yönetme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542037"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="545b3-102">Birincil e-posta adresi ayarlamak veya kullanıcı özniteliklerini değiştirmek için</span><span class="sxs-lookup"><span data-stu-id="545b3-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="545b3-103">Ortamınız için dizin eşitleme etkinse, Microsoft 365 Yönetim Merkezi'ni kullanarak bazı kullanıcı veya nesne öznitelikleri değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="545b3-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="545b3-104">Eşzamanlı kullanıcılar ve tüm öznitelikleriyle tam olarak yönetmek için yerel active directory kullanıcıları ve grupları Yönetimi Konsolu (adsiedit.msc) kullanın.</span><span class="sxs-lookup"><span data-stu-id="545b3-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="545b3-105">Alternatif olarak, tek tek kullanıcılara veya gibi ortak bu örneklerde gösterilen powershell kullanarak eşitlenen kullanıcıların özniteliklerini değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="545b3-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="545b3-106">Kümesi-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="545b3-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="545b3-107">Kümesi-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test" kullanıcı"- Soyadı"Kullanıcı"-"Yönetici"Başlık-bölüm"HR"</span><span class="sxs-lookup"><span data-stu-id="545b3-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="545b3-108">Kaldır-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="545b3-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>