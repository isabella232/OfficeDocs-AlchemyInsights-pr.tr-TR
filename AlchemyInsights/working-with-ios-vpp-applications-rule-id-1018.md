---
title: iOS VPP Uygulamaları ile Çalışma Kural Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719977"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP Uygulamaları ile Çalışma

Apple Toplu Satın Alma Programı'ndan ve Microsoft Intune'da bu programa yönelik destekten yararlanmak için microsoft [Intune ile toplu satın alma programı aracılığıyla satın alınan iOS uygulamalarını nasıl](https://docs.microsoft.com/intune/vpp-apps-ios) yönetebilirsiniz'i okuyun.
  
 **Sık Karşılaşılan Sorunlar:** "Kullanıcılarıma bir iOS VPP uygulaması atadim, ancak yükleme başarısız oldu."
  
- Tek bir VPP belirteci birden çok mobil cihaz yönetim sağlayıcısında kullanılırsa bu durum olabilir. Apple'ın VPP belirteçleri yalnızca tek bir sağlayıcıda kullanılabilir. Birden çok sağlayıcıiçeren bir VPP belirteci kullandıysanız, belirteci Intune'a yeniden yüklemeniz gerekir.

- Toplam yükleme sayısı lisans sayısını aşarsa yükleme de başarısız olabilir. Lisanslarınız için kullanım raporunu görüntülemek için **Intune Mobile uygulamaları** \> **Uygulaması lisansları** sayfasına gidin. Kullanılan lisansları nasıl geri alacağız'u öğrenmek için [bu makaleye bakın.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
