---
title: Apple Otomatik Cihaz Kaydı eşitleme hataları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013768"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple Otomatik Cihaz Kaydı eşitleme hataları

"Hata durumuna sahip bir veya daha fazla ADE/DEP Belirtecimiz olduğunu algıladık. Etkilenen her belirteç için hata durumu çözümleninceye kadar ADE işlevselliği beklendiği gibi çalışmayecektir."

Bu hata çeşitli yollarla ortaya çıkar:

1. Cihazlar ABM/ASM'den Intune'a eşitleney
2. Kayıt profili atamaları başarısız olabilir
3. Cihazlar ADE kaydı başarıyla tamamlanamadı

Intune konsolunda Cihazlar ve Apple kayıt belirteçleri > Cihazları > altında intune **konsolunda bildirilen eşitleme > kontrol edin.**

Eşitleme hatasının en yaygın nedenlerinden biri geçerli belirtecin süresinin dolmasıdır. Birçok durumda, etkilenen belirtecin yenilenmesi sorunu çözer.

Belirteçlerin birinin veya birden fazlasının süresi dolduğunda, bunları uygun şekilde yenilemenize yardımcı olması için aşağıdaki belgelere bakın:

[Otomatik Cihaz Kaydı belirteci yenileme](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Buna ek olarak, belirteç eşitleme hatalarına neden olan diğer hataların olası düzeltmelerini görmek için aşağıdaki belgeleri de bulabilirsiniz:

[iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
