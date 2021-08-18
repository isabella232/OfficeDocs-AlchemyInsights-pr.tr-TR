---
title: Klasik kök sitenizi Modern siteyle değiştirme
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
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316160"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klasik kök sitenizi Modern siteyle değiştirme

Ortamınız Nisan 2019'dan önce ayarlanmışsa, Microsoft PowerShell kullanarak kök siteyi modern bir site olarak değiştirebilirsiniz:

- Kök siteniz olarak kullanmak istediğiniz farklı bir site varsa, kök siteyi siteyle [değiştirebilirsiniz (değiştirebilirsiniz).](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Özgün siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın. Hem Ekip Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir. 

- Yakında, sitenin içeriğini kullanmaya devam etmek ancak var olan siteyi bir iletişim sitesine dönüştürmenizi sağlayacak ek özellikler de yakında yayınlanacak. 

**Önemli:** Bu özellikler aşamalı olarak tüm özelliklere sahip olacak. Güncelleştirmeleri İleti Merkezi'nde denetlemeye devam edin. 

## <a name="known-issues-with-swapping-sites"></a>Site değiştirmeyle ilgili bilinen sorunlar

- Hedef site kısa bir süre için "bulunamadı" (HTTP 404) hatası döndürür.
- Arama dizinini güncelleştirmek için içeriğin yeniden akmış olması gerekir. El ile herhangi bir adım gerekmez; bu işlem otomatik olarak yapılır.
- "Statik" bağlantılara (Dosya Eşitleme ve OneNote gibi) bağımlı olan her şeyin el ile düzeltilmesi gerekir.
- Kaynak site bir kuruluş haber sitesi ise, URL'yi güncelleştirin. Tüm kurumsal haber sitelerinin listesini al.
- Project Hala doğru ilişkilendirillerinden emin olmak için sunucu sitelerinin doğrulanması gerekiyor olabilir.
