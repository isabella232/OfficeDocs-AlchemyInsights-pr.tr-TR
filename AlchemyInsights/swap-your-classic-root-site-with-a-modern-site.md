---
title: Klasik kök sitenizin Modern bir site ile takas
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501099"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasik kök sitenizin Modern bir site ile takas

Ortamınızı önce Nisan 2019 ayarlarsanız, modern bir siteye kök sitenizin Microsoft PowerShell kullanarak değiştirebilirsiniz:

- Sitenizin kök kullanmak istediğiniz farklı bir site varsa, (takas) kök site ile değiştirebilirsiniz. 
    - [Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) konumunu başka bir siteye sahip bir site, özgün site Arşivlerken takas etmek için kullanın. Ekip sitesi (bir gruba bağlı değil) hem de iletişim Site için kullanılabilir. 

- Ek yetenekler kullanılmaya başlanan yakında olanak tanıyacak şekilde sitesindeki içeriği kullanarak tutmak, ancak varolan sitenin iletişim siteye dönüştürmek. 
>[!Important]
>Bu yetenekleri yavaş yavaş piyasaya çıkacağı. Güncelleştirmeler için Office 365 ileti merkezi bakmaya devam edin. 

## <a name="known-issues-with-swapping-sites"></a>Takas siteleri ile ilgili bilinen sorunlar

- Hedef site kısa bir süre için bir "not found" (HTTP 404) hata döndürebilir.
- İçerik arama dizini güncelleştirmek için recrawled gerekecek. Gereken el ile hiçbir adım - bu otomatik olarak yapılacaktır.
- "Statik" bağlantıları (örneğin, dosya eşitleme ve OneNote dosyaları) bağımlı bir şey elle düzeltilmesi gerekir.
- Kaynak site kuruluş haber sitesi varsa, URL'yi güncelleştirin.Tüm kuruluş haber sitelerin bir listesini alın.
- Project Server siteleri doğru hala ilişkili olduklarından emin olmak için doğrulanması gerekebilir.





