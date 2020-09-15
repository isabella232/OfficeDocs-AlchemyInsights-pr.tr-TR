---
title: İOS VPP uygulamalarıyla çalışma kuralı 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688966"
---
# <a name="working-with-ios-vpp-applications"></a>İOS VPP uygulamalarıyla çalışma

Apple Volume Purchase programından ve Microsoft Intune 'da sağlanan desteği kullanmanın özelliklerini, kısıtlamalarını ve adımlarını öğrenmek için, [Microsoft Intune ile bir toplu satın alma programı aracılığıyla satın alınan iOS uygulamalarını yönetmeyi](https://docs.microsoft.com/intune/vpp-apps-ios) okuyun.
  
 **Sık karşılaşılan sorunlar:** "Kullanıcılarıma bir iOS VPP uygulaması atadım, ancak yükleme başarısız oldu."
  
- Birden çok mobil cihaz yönetim sağlayıcısı genelinde tek bir VPP belirteci kullanılıyorsa bu olabilir. Apple 'dan alınan VPP belirteçleri yalnızca bir sağlayıcı ile kullanılabilir. Birden çok sağlayıcı içeren bir VPP belirteci kullandıysanız, belirteci Intune 'a yeniden yüklemelisiniz.

- Toplam yükleme sayısı lisans sayısını aştığında de yükleme başarısız olabilir. Lisanslarınız için kullanım raporunu görüntülemek için **Intune mobil uygulamalar** \> **uygulama lisansları** sayfasına gidin. Lisansları kullanımda geri kazanma hakkında bilgi edinmek için [Bu makaleye bakın.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
