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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448942"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple Otomatik Cihaz Kaydı eşitleme hataları

"Bir veya birden çok ADE/DEP Belirtecinin hata durumuna sahip olduğunu algıladık. Etkilenen her belirteç için hata durumu çözülene kadar ADE işlevi beklendiği gibi çalışmayacak."

Bu hata çeşitli yollarla ortaya çıkar:

1. Cihazlar ABM/ASM'den Intune'a eşitleyene
2. Kayıt profili atamaları başarısız olabilir
3. Cihazlar ADE kaydı başarıyla tamamlanamadı

Intune konsolunda Cihazlar ve Cihazları Kaydetme > Apple kayıt > Kayıt programı belirteçleri > bildirilen eşitleme **hatasını kontrol edin.**

Eşitleme hatasının en yaygın nedenlerinden biri, geçerli belirtecin süresinin dolmasıdır. Çoğu durumda, etkilenen belirtecin yenilenmesi sorunu çözer.

Belirteçlerin birinin veya daha fazlasının süresi dolduğunda, uygun şekilde yenilemenize yardımcı olması için aşağıdaki belgelere bakın:

[Otomatik Cihaz Kaydı belirteci yenileme](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Buna ek olarak, belirteç eşitleme hatalarına neden olan diğer hataların olası düzeltmelerini görmek için aşağıdaki belgeleri de bulabilirsiniz:

[iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
