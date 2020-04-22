---
title: Posta kutusu denetimini etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703591"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="31d22-102">Posta kutusu denetimini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="31d22-102">Enable mailbox auditing</span></span>

<span data-ttu-id="31d22-103">Tek bir kullanıcı veya tüm kuruluş için Posta Kutusu Denetimi'ni etkinleştirmek için Aşağıdaki cmdlets Remote Power Shell'den çalıştırılmalıdır:</span><span class="sxs-lookup"><span data-stu-id="31d22-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="31d22-104">**Tek Kullanıcı**</span><span class="sxs-lookup"><span data-stu-id="31d22-104">**Single User**</span></span>
  
<span data-ttu-id="31d22-105">Set-Mailbox -Kimlik "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="31d22-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="31d22-106">**Organizasyon**</span><span class="sxs-lookup"><span data-stu-id="31d22-106">**Organization**</span></span>
  
<span data-ttu-id="31d22-107">Get-Mailbox -ResultSize Sınırsız -Filtre {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="31d22-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="31d22-108">Daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="31d22-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

