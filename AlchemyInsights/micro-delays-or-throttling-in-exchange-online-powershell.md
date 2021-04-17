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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar

Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz. İşte bununla ilgili iki öneri:

- REST API’yi temel alan ve çok daha yüksek performans gösteren CMDlet’lerin bulunduğu [Exchange Online v2 PowerShell modülünü](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) kullanmak isteyebilirsiniz. Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.
- Henüz v2 modülünün kapsamında olmayan CMDlet’leri kullanmanız gerekirse, Exchange Online’da beklenen PowerShell azaltma sınırlarını aşmanın açıklandığı [Office 365’te çok fazla sayıda kullanıcı için PowerShell cmdlet’leri çalıştırma](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) konusuna bakın.
