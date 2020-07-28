---
title: Kayıp iOS aygıtlarını Intune ile bulma
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440432"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Kayıp iOS aygıtlarını Intune ile bulma

iOS aygıtında kayıp modu etkinleştirmek, yöneticinin kilit ekranında bir ileti ve iletişim telefonu numarasının görüntülenmesine olanak tanır.

Kayıp modu etkinleştirildikten sonra yönetici, aygıtın fiziksel konumunu belirlemek için Cihazı Bul eylemini kullanabilir.

Intune'daki Cihazı Bul eylemi, belirli bir aygıtın konumunu haritada göstermek için iOS aygıtlarıyla birlikte çalışır.

Bu eylemi kullanmak için iOS aygıtının aşağıdakilerde yer alabını gerektirir:

- Denetlenen mod
- Kayıp mod

Daha fazla bilgi için bkz: [Intune ile iOS/iPadOS aygıtlarında kayıp modu etkinleştir](https://docs.microsoft.com/intune/device-lost-mode) ve [Intune ile kaybolan veya çalınan iOS/iPadOS aygıtlarını bulun.](https://docs.microsoft.com/intune/device-locate)

**SSS**

S: Şirket verilerini bir aygıttan kaldırmak için uzaktan bir eylem yayınladım ve şimdi bekleyen bir durumda.

C: Uzaktan eylemin başarıyla tamamlanması için hedeflenen aygıtın çevrimiçi ve sağlıklı olması gerekir. Aşağıdaki durumlarda, uzak eylem 30 gün boyunca bekleme durumunda kalır veya aygıt komutu kabul edene kadar:

- Aygıtın bağlantısı yoksa
- Cihaz Intune ile yönetim durumunu kaybettiğinde

Bir aygıtın artık check-in olmadığını ve şirket verilerini kaldıramayacağını düşünüyorsanız Sil'i seçin. Silme, aygıt kaydını kaldırarak aygıtların Intune listesinde artık görünmeyerek kaldırır. Aygıt yeniden etkin hale gelirse, kullanıcısının yeniden kaydetmesi gerekir.

S: Neden bazı uzak eylemleri kullanmak için kullanılabilir değil mi?

C: Tüm platformlar tüm uzak aygıt eylemlerini desteklemez. Aşağıdaki uzak eylemler platforma özgüdür, bu nedenle yalnızca belirtilen platformlar için kullanılabilir.

- Etkinleştirme Kilidini Atlama (yalnızca iOS)
- Yeni Başlangıç (yalnızca Windows)
- Kayıp modu (yalnızca iOS)
- Aygıtı bulma (yalnızca iOS)
- Yeniden başlat (yalnızca Windows)

Her eylem hakkında daha fazla bilgi için [kullanılabilir aygıt eylemleri'ne](https://docs.microsoft.com/intune/device-management#available-device-actions)bakın.