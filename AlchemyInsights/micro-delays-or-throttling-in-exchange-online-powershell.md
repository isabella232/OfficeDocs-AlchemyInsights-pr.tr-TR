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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830053"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="6c7ea-102">Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar</span><span class="sxs-lookup"><span data-stu-id="6c7ea-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="6c7ea-103">Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6c7ea-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="6c7ea-104">İşte bununla ilgili iki öneri:</span><span class="sxs-lookup"><span data-stu-id="6c7ea-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="6c7ea-105">REST API’yi temel alan ve çok daha yüksek performans gösteren CMDlet’lerin bulunduğu [Exchange Online v2 PowerShell modülünü](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) kullanmak isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6c7ea-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="6c7ea-106">Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.</span><span class="sxs-lookup"><span data-stu-id="6c7ea-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="6c7ea-107">Henüz v2 modülünün kapsamında olmayan CMDlet’leri kullanmanız gerekirse, Exchange Online’da beklenen PowerShell azaltma sınırlarını aşmanın açıklandığı [Office 365’te çok fazla sayıda kullanıcı için PowerShell cmdlet’leri çalıştırma](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="6c7ea-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
