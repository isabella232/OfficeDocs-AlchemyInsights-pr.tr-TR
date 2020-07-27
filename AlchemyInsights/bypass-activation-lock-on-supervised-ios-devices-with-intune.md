---
title: Intune ile denetlenen iOS aygıtlarında etkinleştirme kilidini atlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424209"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Intune ile denetlenen iOS aygıtlarında etkinleştirme kilidini atlama

iOS aygıtlarında etkinleştirme kilidini atlayabilmesi, kullanıcının bir şirket aygıtında etkinleştirme kilidini etkinleştirdiği ve ardından şirketten ayrıldığı senaryodan kurtulmayı kolaylaştırır.

Etkinleştirme kilidini atlamak için ön koşullar şunlardır:

- "Denetlenen" bir aygıttır.
- Etkinleştirme kilidi, Intune'da iOS Aygıt kısıtlama ilkesi kullanılarak başarıyla etkinleştirilir.

Ayrıca, etkinleştirme kilidini atlarken şunları

- Fiziksel olarak silinen cihaza sahip.
- Silmeyi vermeden önce kodu kopyalayın.

**Not:** Silme kodu büyük/küçük harf duyarlı değildir, bu nedenle "-" karakterler gerekli değildir.

Ayrıntılar için, [Intune'a sahip Denetlenen iOS aygıtlarında Etkinleştirme Kilidini Bypass'a](https://docs.microsoft.com/intune/device-activation-lock-bypass)bakın.

**SSS**

S: **Şirket verilerini bir aygıttan kaldırmak için uzaktan bir eylem yayınladım ve şimdi bekleyen bir durumda.**

C: Uzaktan eylemin başarıyla tamamlanması için hedeflenen aygıtın çevrimiçi ve sağlıklı olması gerekir. Aşağıdaki durumlarda, uzak eylem 30 gün boyunca bekleme durumunda kalır veya aygıt aşağıdaki durumlarda komutu kabul edene kadar:

- Bağlantı yok.
- Intune ile yönetim statüsünü kaybeder.

Aygıtın artık check-in olmadığını ve şirket verilerini kaldırmayacağını düşünüyorsanız Sil'i seçin. Silme, aygıt kaydını kaldırarak aygıtların Intune listesinde artık görünmeyerek kaldırır. Aygıtın yeniden etkin hale gelmesi için, kullanıcının aygıtı yeniden kaydetmesi gerekir.

S: **Neden bazı uzak eylemleri kullanmak için kullanılabilir değil mi?**

C: Tüm platformlar tüm uzak aygıt eylemlerini desteklemez. Aşağıdaki uzak eylemler platforma özgüdür.

- Etkinleştirme Kilidini Atlama (yalnızca iOS)
- Yeni Başlangıç (yalnızca Windows)
- Kayıp modu (yalnızca iOS)
- Aygıtı bulma (yalnızca iOS)
- Yeniden başlat (yalnızca Windows)

Her eylem hakkında daha fazla bilgi için [kullanılabilir aygıt eylemleri'ne](https://docs.microsoft.com/intune/device-management#available-device-actions)bakın.