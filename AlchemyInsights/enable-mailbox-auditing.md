---
title: Posta kutusu denetimini etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806311"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="9d9f0-102">Posta kutusu denetimini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="9d9f0-102">Enable mailbox auditing</span></span>

<span data-ttu-id="9d9f0-103">Tek bir kullanıcı veya kuruluşun tamamında posta kutusu denetimini etkinleştirmek için, aşağıdaki cmdlet 'lerin uzak Power Shell 'den çalıştırılması gerekir:</span><span class="sxs-lookup"><span data-stu-id="9d9f0-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="9d9f0-104">**Tek Kullanıcı**</span><span class="sxs-lookup"><span data-stu-id="9d9f0-104">**Single User**</span></span>
  
<span data-ttu-id="9d9f0-105">Set-Mailbox-Identity "Gamze"-Sestenabled $true</span><span class="sxs-lookup"><span data-stu-id="9d9f0-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="9d9f0-106">**Kuruluşunu**</span><span class="sxs-lookup"><span data-stu-id="9d9f0-106">**Organization**</span></span>
  
<span data-ttu-id="9d9f0-107">Get-posta kutusu-ResultSize Sınırsız filtre {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-Sestenabled $true</span><span class="sxs-lookup"><span data-stu-id="9d9f0-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="9d9f0-108">Daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="9d9f0-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

