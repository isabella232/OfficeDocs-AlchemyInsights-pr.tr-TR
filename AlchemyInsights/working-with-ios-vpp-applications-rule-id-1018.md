---
title: iOS VPP Uygulamaları Kural Kimliği 1018 ile çalışma
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083034"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP Uygulamaları ile çalışma

Apple Toplu Satın Alma Programı'nın kullanımı ve Microsoft Intune'de bu programı desteklemeye yardımcı olacak özellikler, kısıtlamalar ve adımlar hakkında bilgi edinmek için Microsoft Intune ile bir satın alma programı aracılığıyla satın alınan [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) uygulamalarını yönetme Microsoft Intune.
  
 **Sık Karşılaşılan Sorunlar:** "Kullanıcılarıma bir iOS VPP uygulaması atadı, ancak yükleme başarısız oldu."
  
- Birden çok mobil cihaz yönetim sağlayıcısında tek bir VPP belirteci kullanılıyorsa bu durumla karşı karşıya olun. Apple'ın VPP belirteçleri yalnızca bir sağlayıcıyla kullanılabilir. Birden çok sağlayıcıyla VPP belirteci kullandıysanız, belirteci Intune'a yeniden yükley seçmelisiniz.

- Toplam yükleme sayısı lisans sayısını aşarsa da yükleme başarısız olabilir. Lisanslarınızı kullanım raporunu görüntülemek için **Intune Mobil** uygulamaları Uygulama lisansları \> **sayfasına** gidin. Kullanım lisanslarını geri almak için bu [makaleye bakın.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
