---
title: Defender Endpoint check sensor status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676543"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint check sensor status

Algılayıcı **sorunu olan cihazlar kutucuğu** Güvenlik İşlemleri panosunda bulunur. Bu kutucuk, ayrı ayrı cihazın algılayıcı verilerini sağlayabilme ve Uç Nokta için Defender hizmetiyle iletişim kurma özelliği hakkında bilgi sağlar. Bu rapor, kaç cihazla dikkat gerektir olduğunu rapor etmektedir ve sorunlu cihazları tanımları ve bilinen sorunları düzeltmeye yardımcı olur.

Kutucukta yer alan iki durum göstergesi, hizmete düzgün bir şekilde rapornabilecek cihaz sayısı hakkında bilgi sağlar:

- **Hatalı Yapılandırılmış** Kısmen algılayıcı verilerini Uç Nokta için Defender hizmetine bildiren ve düzeltilmesi gereken yapılandırma hataları olan cihazlar.
- **Etkin değil** Geçen ay yediden fazla gün boyunca Uç Nokta için Defender hizmetine bildirmeyi durduran cihazlar.

Gruplardan herhangi birini tıklatmak sizi seçeneklere göre filtrelenmiş olarak Cihazlar listesine yönlendirmektedir. Cihazlar listesinde durum listesini aşağıdaki durum durumuna göre filtre yapabilirsiniz:

- **Etkin** Etkin olarak Uç nokta için Defender hizmetine rapor yapan cihazlar.
- **Hatalı Yapılandırılmış** Kısmen algılayıcı verilerini Uç Nokta için Defender hizmetine bildiriyor ama düzeltilmesi gereken yapılandırma hataları olan cihazlar. Yanlış yapılandırılmış cihazlar aşağıdaki sorunlardan birini veya bir birleşimine sahip olabilir:

    - Algılayıcı verisi yok - Cihazlar algılayıcı verilerini göndermeyi durdurdu. Cihazdan sınırlı uyarılar tetiklenir.
    - İletişim engelli - Cihazla iletişim kurma yeteneği engellidir. Daha derin çözümleme yapmak, dosyaları engellemek, cihazı ağdan ve cihazla iletişim gerektiren diğer eylemlerden göndermek işe yaramadı.
- **Etkin değil** Uç nokta için Defender hizmetine bildirmeyi durduran cihazlar.

Dışarı Aktar özelliğini kullanarak listenin tamamını CSV biçiminde indirebilirsiniz.

Daha fazla bilgi için [bkz. Uç Nokta için Microsoft Defender'da algılayıcıların durumunu denetleme.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Bir cihazın devre dışı veya hatalı yapılandırılmasına neyin neden olduğu hakkında daha fazla bilgi için bkz. Uç Nokta için Microsoft Defender'daki uygun olmayan [algılayıcıları düzeltme](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
