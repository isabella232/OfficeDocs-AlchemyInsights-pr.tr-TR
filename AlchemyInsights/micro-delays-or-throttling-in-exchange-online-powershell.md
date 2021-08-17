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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314720"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar

Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz. Bunu çözmek için birkaç önerimiz var:

- Kiracınızı PowerShell azaltma ilkelerini rahatlatk için lütfen tanılamalarımızı çalıştırın. Bu çözüm sorunu en çok çözer.
- Sorun yine de çözülmezse, REST API'sini temel alan ve çok daha iyi performans ortaya konulan CMDlet'leri içeren [v2 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modülünü kullanın. Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.
- v2 modülünde yer almayan CMDlet'leri kullanmak zorundaysanız, lütfen Office 365'ta çok sayıda kullanıcı için [PowerShell cmdlet'lerini](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)çalıştırma 'ya bakın. Bu cmdlet'ler, Exchange Online'te PowerShell azaltma sınırlarını aşmayı ele Exchange Online.
