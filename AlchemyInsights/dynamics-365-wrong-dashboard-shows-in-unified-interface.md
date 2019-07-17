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
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749039"
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
