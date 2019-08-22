---
title: Dynamics 365 - yanlış Pano Dynamics 365 birleştirilmiş arabiriminde gösterilir.
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528571"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Yanlış Pano Dynamics 365 birleştirilmiş arabiriminde gösterilir.

Neden beklediğiniz olandan farklı bir Pano görebilirsiniz çeşitli nedenleri vardır:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kullanıcı bir kullanıcı varsayılan pano ayarladı. 

Bir kullanıcıyı tanımlamak genellikle varsayılan pano ayarlanmışsa Pano komut çubuğunda **Varsayılan olarak belirle** düğmesini göstermez. Kullanıcının varsayılan pano içinde geçerli app olmasa bile, kullanıcı varsayılan pano diğer varsayılan panolar geçersiz kılar.

Kendi varsayılan Pano için unset aşağıdaki geçici çözümü kullanın.

1. Yeni bir kişisel pano oluşturun.

2. Yeni bir pano, kullanıcı varsayılan olarak ayarlayın.

3. Bu panoyu silme.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pano Site Haritası ayarlanır

Bir Pano seçerek ve 'Varsayılan olarak belirle' altında 'Sistem Özelleştirme' seçme, bir kuruluşun varsayılan pano ayarlamış olabilirsiniz. Ancak, kullanıcı erişimi varsa, site haritası Tasarımcısı'nda tanımlanan Pano bu pano üzerinde öncelik kazanır.

Kullanıcıların kuruluş varsayılan olarak ayarladığınız Pano görmek için aşağıdakileri yapabilirsiniz:

* Bu Pano Site Haritası içinde ayarlama

* Sitemap tanımlı Pano kullanıcılar için erişimi kaldırmak
