---
title: Windows 10'da sürücü alanı boş bırak
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037952"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10'da sürücü alanı boş bırak

Windows'da sürücü alanı için iki seçenek vardır:

- Windows 10'da sürücü alanınız için boş alan sağlar.
- Dış depolama cihazıyla Windows 10 güncelleştirmeleri için yer açın.

Disk Temizleme'yi kullandıktan sonra disk alanınız hala düşükse, Temp klasörünüz Microsoft Store tarafından kullanılan uygulama (.appx) dosyalarıyla hızla dolduruluyor olabilir. Bu sorunu çözmek için Mağaza'yı sıfırlayın, Mağaza önbelleğini temizleyin ve Windows Update sorun gidericisini çalıştırın. Bu adımlarla devammeden önce Microsoft Store'un kapalı olduğundan emin olun.

**1. Adım: Microsoft Store'u sıfırlama**

**Not** Bu, tercihleriniz ve oturum açma ayrıntıları da dahil olmak üzere cihaz üzerinde uygulama verilerini kalıcı olarak siler.

1. Başlangıç **Ayarları**  >  **Uygulamaları**  >  **uygulamaları**&  >  **seçin.**

1. Uygulama listesinde Microsoft Store'u bulun ve seçin.

1. Gelişmiş **seçenekleri belirleyin.**

1. Aşağı kaydırın ve **Sıfırla'yı seçin** ve sonra Sıfırlamayı **Onayla'yı seçin.**

**2. Adım: Microsoft Store önbelleğini temizleme**

1. Çalıştır iletişim kutusunu açmak için Windows Logo Tuşu + R tuşlarına basın.

1. Arama wsreset.exe Tamam'ı **seçin.**

1. Boş bir Komut İstemi penceresi açılır. Yaklaşık 10 saniye sonra pencere kapanır ve Mağaza otomatik olarak açılır.

**3. Adım: Windows Update'i sıfırlama**

1. Güvenlik **Sorunlarını**  >  **Gidermek**  >  **için Ayarlar &'ni**  >  **seçin.**

1. Aşağı kaydırın ve **listeden Windows Update'i** seçin ve sorun **gidericiyi çalıştır'ı seçin.**

1. Bilgisayarınızı yeniden başlatın ve sorunu hala yaşıyor olup olmadığınızı kontrol edin.

