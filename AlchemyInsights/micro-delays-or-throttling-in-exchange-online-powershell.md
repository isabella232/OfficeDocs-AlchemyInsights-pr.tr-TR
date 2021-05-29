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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar

Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz. Bunu çözmek için birkaç önerimiz var:

- Kiracınızı PowerShell azaltma ilkelerini rahatlatk için lütfen tanılama yöntemlerimizi çalıştırın. Bu çözüm sorunu en çok çözer.
- Sorun yine de çözülmezse, REST API'sini temel alan ve önemli ölçüde performansa sahip cmDlet'leri içeren Exchange Online [v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modülünü kullanın. Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.
- v2 modülünde yer almayan CMDlet'leri kullanmak zorundaysanız, lütfen Office 365'ta çok sayıda kullanıcı için [PowerShell cmdlet'lerini](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)çalıştırma 'ya bakın. Bu cmdlet'ler, Exchange Online'te PowerShell azaltma sınırlarını aşmayı ele Exchange Online.
