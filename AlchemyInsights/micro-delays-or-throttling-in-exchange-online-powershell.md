---
title: Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702146"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="0b024-102">Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar</span><span class="sxs-lookup"><span data-stu-id="0b024-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="0b024-103">Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0b024-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="0b024-104">Bunu çözmek için birkaç önerimiz var:</span><span class="sxs-lookup"><span data-stu-id="0b024-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="0b024-105">Kiracınızı PowerShell azaltma ilkelerini rahatlatk için lütfen tanılama yöntemlerimizi çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="0b024-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="0b024-106">Bu çözüm sorunu en çok çözer.</span><span class="sxs-lookup"><span data-stu-id="0b024-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="0b024-107">Sorun yine de çözülmezse, REST API'sini temel alan ve önemli ölçüde performansa sahip cmDlet'leri içeren Exchange Online [v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modülünü kullanın.</span><span class="sxs-lookup"><span data-stu-id="0b024-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="0b024-108">Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.</span><span class="sxs-lookup"><span data-stu-id="0b024-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="0b024-109">v2 modülünde yer almayan CMDlet'leri kullanmak zorundaysanız, lütfen Office 365'ta çok sayıda kullanıcı için [PowerShell cmdlet'lerini](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)çalıştırma 'ya bakın. Bu cmdlet'ler, Exchange Online'te PowerShell azaltma sınırlarını aşmayı ele Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0b024-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
