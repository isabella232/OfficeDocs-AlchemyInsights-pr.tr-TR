---
title: Posta kutusu denetimini etkinleştirme
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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736273"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="cbf78-102">Posta kutusu denetimini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="cbf78-102">Enable mailbox auditing</span></span>

<span data-ttu-id="cbf78-103">Tek bir kullanıcı veya tüm kuruluş için Posta Kutusu Denetimi'ni etkinleştirmek için Aşağıdaki cmdlets Remote Power Shell'den çalıştırılmalıdır:</span><span class="sxs-lookup"><span data-stu-id="cbf78-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="cbf78-104">**Tek Kullanıcı**</span><span class="sxs-lookup"><span data-stu-id="cbf78-104">**Single User**</span></span>
  
<span data-ttu-id="cbf78-105">Set-Mailbox -Kimlik "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cbf78-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="cbf78-106">**Organizasyon**</span><span class="sxs-lookup"><span data-stu-id="cbf78-106">**Organization**</span></span>
  
<span data-ttu-id="cbf78-107">Get-Mailbox -ResultSize Sınırsız -Filtre {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cbf78-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="cbf78-108">Daha fazla bilgi edinin</span><span class="sxs-lookup"><span data-stu-id="cbf78-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

