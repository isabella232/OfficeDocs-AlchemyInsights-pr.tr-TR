---
title: Dynamics 365-Dynamics 365 Birleşik arabiriminde yanlış Pano gösteriliyor
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711295"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 Birleşik arabiriminde yanlış Pano gösteriliyor

Beklediğinizden farklı bir panoyu görmenizin birkaç nedeni vardır:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kullanıcı varsayılan kullanıcı panosunu ayarladı 

Genellikle, **Varsayılan olarak ayarla** düğmesi Pano komut çubuğunda görünmüyorsa, Kullanıcı varsayılan panosunun ayarlandığını belirleyebilirsiniz. Kullanıcının varsayılan panosu geçerli uygulamada olmasa bile, Kullanıcı varsayılan panosu tüm diğer varsayılan panoları geçersiz kılar.

Varsayılan panosunu atamak için aşağıdaki geçici çözümü kullanın.

1. Yeni bir kişisel pano oluşturun.

2. Yeni panoyu Kullanıcı varsayılanı olarak ayarlayın.

3. Panoyu silin.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pano Site Haritası 'nda ayarlanır

Bir panoyu seçip ' Sistemi Özelleştir ' altında ' varsayılan olarak ayarla ' seçeneğini belirleyerek bir kuruluşun varsayılan panosunu ayarlamış olabilirsiniz. Ancak site haritası tasarımcısında tanımlanan Pano bu panoyu, kullanıcının erişimi varsa bu panoda önceliklidir.

Kullanıcıların kuruluş varsayılanı olarak ayarlamış olduğunuz panoyu görmesi için şunları yapabilirsiniz:

* Bu panoyu site haritası 'nda ayarlama

* Bu kullanıcılar için site haritası tanımlı panoya erişimi kaldırma
