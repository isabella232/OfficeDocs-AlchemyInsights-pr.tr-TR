---
title: Klasik kök sitenizi modern bir siteyle değiştirme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691199"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasik kök sitenizi modern bir siteyle değiştirme

Ortamınız 2019 Nisan 'dan önce ayarlanmışsa, Microsoft PowerShell kullanarak kök sitenizi modern bir siteye dönüştürebilirsiniz:

- Kök siteniz olarak kullanmak istediğiniz farklı bir siteniz varsa, [kök siteyi onunla değiştirebilirsiniz (takas edebilirsiniz)](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Özgün siteyi arşivlerken, bir sitenin konumunu başka bir siteyle değiştirmek için [çağır-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 'ı kullanın. Hem ekip sitesi (gruba bağlı değil) hem de Iletişim sitesi için kullanılabilir. 

- Sitedeki içeriği kullanmaya devam edecek ancak var olan siteyi bir iletişim sitesine dönüştürebilecek olan ek özellikler yakında kullanıma sunulacaktır. 
>[!Important]
>Bu özellikler aşamalı olarak kullanıma sunulacaktır. Güncelleştirmelerin Ileti merkezini denetlemeye devam edin. 

## <a name="known-issues-with-swapping-sites"></a>Siteleri değiştirme ile ilgili bilinen sorunlar

- Hedef site kısa bir süre boyunca "bulunamadı" (HTTP 404) hatası döndürebilir.
- İçerik, arama dizinini güncelleştirmek için yeniden gezilecek. El ile adım gerekmez; Bu işlem otomatik olarak yapılır.
- "Statik" bağlantılara (dosya eşitleme ve OneNote dosyaları gibi) bağlı olarak, el ile düzeltilmesi gerekir.
- Kaynak site bir kuruluş haber sitesidir, URL 'YI güncelleyin.Tüm kuruluş haberleri sitelerinin listesini alın.
- Project Server sitelerinin doğru ilişkilendirilmeleri için doğrulanması gerekebilir.
