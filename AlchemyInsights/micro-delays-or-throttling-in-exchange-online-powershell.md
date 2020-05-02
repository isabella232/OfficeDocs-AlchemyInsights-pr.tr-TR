---
title: Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948027"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell’de küçük gecikmeler veya azaltmalar

Exchange Online’da betikler ve cmdlet’ler çalıştırırken "Küçük bir gecikme uygulandı" uyarıları veya gecikmeler görebilirsiniz. İşte bununla ilgili iki öneri:

- REST API’yi temel alan ve çok daha yüksek performans gösteren CMDlet’lerin bulunduğu [Exchange Online v2 PowerShell modülünü](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) kullanmak isteyebilirsiniz. Sık kullanılan birçok Get- CMDlet betiği için bu harika bir çözüm olabilir.
- Henüz v2 modülünün kapsamında olmayan CMDlet’leri kullanmanız gerekirse, Exchange Online’da beklenen PowerShell azaltma sınırlarını aşmanın açıklandığı [Office 365’te çok fazla sayıda kullanıcı için PowerShell cmdlet’leri çalıştırma](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) konusuna bakın.
