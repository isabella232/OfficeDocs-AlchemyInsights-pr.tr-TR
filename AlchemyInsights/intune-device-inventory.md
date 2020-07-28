---
title: Intune Cihaz Envanteri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440480"
---
# <a name="intune-device-inventory"></a>Intune Cihaz Envanteri

Cihazlar bıçağı, intune'da yönetim altındaki aygıtlar için yönetici içgörüsü sağlar. Gösterilen bilgiler şunları içerir: Donanım, Keşfedilen uygulamalar, Aygıt Uyumluluğu durumu ve Aygıt Yapılandırma durumu.

Donanım ve keşfedilen uygulamalar için envanter verileri yedi günlük bir döngüde toplanır. Bildirilen uygulamaların ve bildirilen donanımın belirli öğeleri, aygıt işletim sistemine ve cihazın kişisel veya kurumsal sahip olup olmadığına bağlı olarak farklılık gösterir.

Daha fazla bilgi için Bkz. [Intune'daki cihaz ayrıntılarını görün.](https://docs.microsoft.com/intune/device-inventory)

**SSS**

S: Intune kayıtlı Windows aygıtlarında bulunan uygulamaların tam bir envanter listesini almıyorum. Neden olmasın?

C: Şu anda, yalnızca modern uygulamalar kurumsal aygıtlar olarak tanımlanan Windows 10 bilgisayarları için listelenmiştir. Intune, bu cihazlarda yüklü olan Win32 uygulamaları hakkında bilgi toplamaz.

S: Telefon numaraları neden tüm cihazlardan toplanmaz?

C: Intune'da kurumsal aygıt olarak sınıflandırılan telefonlar, örneğin bir mobil cihaz envanter raporu çalıştırdığınızda tam telefon numarasıyla tanımlanmaz. Bring-you-own-kendi cihaz telefon numaraları her zaman kısmen yıldız işaretleri (****) ile maskeli ve yalnızca son dört basamak gösterir.