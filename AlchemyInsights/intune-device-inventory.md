---
title: Intune cihaz stoğu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667898"
---
# <a name="intune-device-inventory"></a>Intune cihaz stoğu

Cihazlar Blade, cihaz temelinde, Intune 'da yönetim 'in altındaki aygıtlara fikir sağlar. Gösterilen bilgiler: donanım, bulunan uygulamalar, cihaz uyumluluk durumu ve cihaz yapılandırma durumu.

Donanım için envanter verileri ve bulunan uygulamalar, yedi günlük döngüde toplanır. Uygulamalar ve belirli donanım öğeleri, cihaz işletim sistemine bağlı olarak ve cihazın kişisel veya şirket sahibi olup olmadığı fark edilir.

Daha fazla bilgi için bkz [.](https://docs.microsoft.com/intune/device-inventory)

**SSS**

S: Intune kayıtlı Windows cihazlarında tüm uygulamaların tam envanter listesini almıyorum. Neden olmasın?

A: Şu anda yalnızca modern uygulamalar, kurumsal cihazlar olarak tanımlanan Windows 10 bilgisayarlarında listelenir. Intune, bu cihazlarda yüklü Win32 uygulamaları hakkında bilgi toplamaz.

S: telefon numaraları neden tüm cihazlardan toplanmadı?

A: Örneğin, bir mobil cihaz envanter raporu çalıştırırsanız, Intune 'da şirket cihazları olarak kategorilere ayrılan telefonlar tam telefon numarasıyla tanımlanmayabilir. Yanınızda getirin-kendi-cihaz telefon numaraları her zaman yıldız işareti (* * * *) ile kısmen maskelenir ve yalnızca son dört basamağı gösterir.