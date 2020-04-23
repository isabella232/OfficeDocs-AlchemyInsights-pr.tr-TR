---
title: Klasik kök sitenizi Modern bir siteyle değiştirin
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741564"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasik kök sitenizi Modern bir siteyle değiştirin

Ortamınız Nisan 2019'dan önce ayarlanmışsa, Microsoft PowerShell'i kullanarak kök sitenizi modern bir siteyle değiştirebilirsiniz:

- Kök siteniz olarak kullanmak istediğiniz farklı bir siteniz varsa, kök siteyi onunla değiştirebilir [(değiştirebilirsiniz).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Orijinal siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın. Hem Takım Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir. 

- Sitedeki içeriği kullanmaya devam etmenizi, ancak varolan siteyi bir iletişim sitesine dönüştürmenizi sağlayacak ek özellikler yakında sunulacaktır. 
>[!Important]
>Bu yetenekler kademeli olarak kullanıma sunulacaktır. Güncelleştirmeler için İleti Merkezi'ni denetlemeye devam edin. 

## <a name="known-issues-with-swapping-sites"></a>Siteleri değiştirme yle ilgili bilinen sorunlar

- Hedef site kısa bir süre için bir "bulunamadı" (HTTP 404) hatası döndürebilir.
- Arama dizinini güncelleştirmek için içeriğin yeniden taranması gerekir. El ile adım gerekmez - bu otomatik olarak yapılacaktır.
- "Statik" bağlantılara (Dosya Eşitlemi ve OneNote dosyaları gibi) bağlı olan her şeyin el ile düzeltilmesi gerekir.
- Kaynak site bir kuruluş haber sitesiyse, URL'yi güncelleştirin.Tüm organizasyonel haber sitelerinin listesini alın.
- Project Server sitelerinin hala doğru ilişkili olduğundan emin olmak için doğrulanması gerekebilir.
