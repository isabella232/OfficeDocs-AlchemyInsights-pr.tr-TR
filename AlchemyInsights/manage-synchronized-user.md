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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380525"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="e86dc-102">Birincil e-posta adresi ayarlamak veya kullanıcı özniteliklerini değiştirmek için</span><span class="sxs-lookup"><span data-stu-id="e86dc-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="e86dc-103">Ortamınız için dizin eşitleme etkinse, bazı kullanıcı veya nesne özniteliklerini Yönetim Merkezi'ni kullanarak değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="e86dc-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="e86dc-104">Eşzamanlı kullanıcılar ve tüm öznitelikleriyle tam olarak yönetmek için yerel active directory kullanıcıları ve grupları Yönetimi Konsolu (adsiedit.msc) kullanın.</span><span class="sxs-lookup"><span data-stu-id="e86dc-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e86dc-105">Alternatif olarak, tek tek kullanıcılara veya gibi ortak bu örneklerde gösterilen powershell kullanarak eşitlenen kullanıcıların özniteliklerini değiştirebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e86dc-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="e86dc-106">Kümesi-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e86dc-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="e86dc-107">Kümesi-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test" kullanıcı"- Soyadı"Kullanıcı"-"Yönetici"Başlık-bölüm"HR"</span><span class="sxs-lookup"><span data-stu-id="e86dc-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="e86dc-108">Kaldır-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e86dc-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>