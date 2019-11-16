---
title: Dynamics 365 - Dynamics 365 Birleşik Arabiriminde Yanlış Pano Gösterir
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528571"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 birleşik arabiriminde yanlış pano gösterir

Beklediğiniz panodan farklı bir pano görmenizin birkaç nedeni vardır:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kullanıcı varsayılan pano belirledi 

Genellikle varsayılan **olarak ayarlı** bir kullanıcı varsayılan panosu nu tanımlayabilirsiniz, pano komut çubuğunda varsayılan olarak ayarlanmaz. Kullanıcı varsayılan panosu, kullanıcının varsayılan panosu geçerli uygulamada olmasa bile diğer tüm varsayılan panoları geçersiz kılar.

Varsayılan panolarını ayarlamak için aşağıdaki geçici çözüme göre kullanın.

1. Yeni bir kişisel pano oluşturun.

2. Yeni panoyu kullanıcı varsayılanı olarak ayarlayın.

3. Şu panoyonu sil.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pano site haritasında ayarlanır

Bir pano seçip 'Sistemi Özelleştir' altında 'Varsayılan Olarak Ayarla' seçeneğini seçerek bir kuruluş varsayılan panosu ayarlamış olabilirsiniz. Ancak, site haritası tasarımcısında tanımlanan pano, kullanıcının bu panoya erişimi varsa, bu panodan önce gelir.

Kullanıcıların ayarladığınız panoyu kuruluş varsayılanı olarak görmesini sağlamak için şunları yapabilirsiniz:

* Site haritasındaki panoyu ayarlama

* Bu kullanıcılar için site haritası tanımlı panoya erişimi kaldırma
