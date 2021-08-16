---
title: Dynamics 365 - Dynamics 365 Birleşik Arabiriminde Yanlış Pano Gösterileri
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101502"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 birleşik arabiriminde yanlış pano görüntüleniyor

Beklediğinizden farklı bir pano görmenin çeşitli nedenleri vardır:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kullanıcı bir kullanıcı varsayılan panosu ayarladi 

Normalde, pano komut çubuğunda Varsayılan Olarak Ayarla düğmesi göster **yoksa,** kullanıcı varsayılan panosu tanımlayabilirsiniz. Kullanıcının varsayılan panosu geçerli uygulamada yermasa bile, kullanıcı varsayılan panosu diğer tüm varsayılan panoları geçersiz kılar.

Varsayılan panolarını geri almak için aşağıdaki geçici çözümü kullanın.

1. Yeni bir kişisel pano oluşturun.

2. Bu yeni panoyu kullanıcı varsayılanı olarak ayarlayın.

3. Panoyu silin.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pano site haritasında ayarlanır

Bir panoyu seçerek ve 'Sistemi Özelleştir' altında 'Varsayılan Olarak Ayarla' öğesini seçerek bir kuruluş varsayılan panosu ayarlayabilirsiniz. Ancak site haritası tasarımcısında tanımlanan pano, kullanıcının erişimi varsa bu panodan öncelikli olacaktır.

Kullanıcıların, kuruluş varsayılanı olarak ayar panoyu görmelerini için, şunları yapabilirsiniz:

* Site haritasında o panoyu ayarlama

* Bu kullanıcılar için site haritası tanımlı panoya erişimi kaldırma
