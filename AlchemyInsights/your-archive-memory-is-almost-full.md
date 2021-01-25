---
title: Arşiv posta kutunuz neredeyse dolu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974667"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="e7bea-102">Arşiv posta kutunuz neredeyse dolu</span><span class="sxs-lookup"><span data-stu-id="e7bea-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="e7bea-103">Kullanıcı uyarıyı alırsa; **Arşiv posta kutunuz neredeyse dolu** veya arşiv posta kutularının boyutunu artırmanız gerekirse, burada bazı ipuçları verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="e7bea-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="e7bea-104">Kullanıcıya Exchange Online Plan 1 atanmışsa, 50 GB 'den 100GB'A kadar olan boyutu yükseltmek için **Exchange Online Plan 2** lisansına yükseltin.</span><span class="sxs-lookup"><span data-stu-id="e7bea-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="e7bea-105">Kullanıcıya aşağıdakilerden herhangi biri atanmış durumda: Exchange Online arşivleme eklentisi ile Exchange **Online Plan 2** veya Exchange Online Plan 1, otomatik genişletme arşivleme özelliğini etkinleştirmek için aşağıdaki adımları kullanın:.</span><span class="sxs-lookup"><span data-stu-id="e7bea-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="e7bea-106">[Exchange Online PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e7bea-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="e7bea-107">Kullanıcıya aşağıdaki komutu bırakın:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="e7bea-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="e7bea-108">Aşağıdaki komutu çalıştırıp Kullanıcı için etkinleştirildiğini doğrulayın:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="e7bea-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="e7bea-109">Daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="e7bea-109">For more information see:</span></span>

- [<span data-ttu-id="e7bea-110"> Sınırsız arşivlemeyi etkinleştir-Yönetici Yardımı-Microsoft 365 uyumluluğu | Microsoft belgeleri</span><span class="sxs-lookup"><span data-stu-id="e7bea-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="e7bea-111">Exchange Online sınırları-hizmet açıklamaları | Microsoft belgeleri</span><span class="sxs-lookup"><span data-stu-id="e7bea-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="e7bea-112">Farklı bir iş planına yükselt | Microsoft belgeleri</span><span class="sxs-lookup"><span data-stu-id="e7bea-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

