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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868554"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar

Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz. Bunu çözmek için birkaç önerimiz var:

- Kiracınızı PowerShell azaltma ilkelerini rahatlatk için lütfen tanılamalarımızı çalıştırın. Bu çözüm sorunu en çok çözer.
- Sorun yine de çözülmezse, REST API'sini temel alan ve önemli ölçüde performansa sahip cmDlet'leri içeren [v2 Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modülünü kullanın. Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.
- v2 modülünde yer almayan CMDlet'leri kullanmak zorundaysanız, lütfen Office 365'ta çok sayıda kullanıcı için [PowerShell cmdlet'lerini](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)çalıştırma 'ya bakın. Bu cmdlet'ler, Exchange Online'te PowerShell azaltma sınırlarını nasıl aşacağız?
