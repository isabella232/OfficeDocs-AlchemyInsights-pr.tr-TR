---
title: Posta kutusu denetimi etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757838"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="1bbf1-102">Posta kutusu denetimi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="1bbf1-102">Enable mailbox auditing</span></span>

<span data-ttu-id="1bbf1-103">Tek bir kullanıcı veya tüm kuruluş için posta kutusu denetimini etkinleştirmek için aşağıdaki cmdlet'leri uzak güç kabuğundan çalıştırmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="1bbf1-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="1bbf1-104">**Tek kullanıcı**</span><span class="sxs-lookup"><span data-stu-id="1bbf1-104">**Single User**</span></span>
  
<span data-ttu-id="1bbf1-105">Set-posta kutusu - kimlik "Jane Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1bbf1-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="1bbf1-106">**Kuruluş**</span><span class="sxs-lookup"><span data-stu-id="1bbf1-106">**Organization**</span></span>
  
<span data-ttu-id="1bbf1-107">Get-posta kutusu - ResultSize sınırsız - filtre {RecipientTypeDetails - eq "UserMailbox"} | Set-posta kutusu - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1bbf1-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="1bbf1-108">Daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="1bbf1-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

