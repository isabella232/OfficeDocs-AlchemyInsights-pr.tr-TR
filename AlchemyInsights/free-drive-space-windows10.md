---
title: Windows 10’da sürücüde boş alan oluşturma
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505376"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10’da sürücüde boş alan oluşturma

Windows’da sürücüde boş alan oluşturmak için iki seçenek vardır:

- Windows 10’da sürücüde boş alan oluşturun.
- Dış depolama cihazı kullanarak Windows 10 güncelleştirmeleri için boş alan oluşturun.

Disk Temizleme aracını kullandıktan sonra disk alanınız hala yetersizse, Temp klasörünüz Microsoft Store tarafından kullanılan uygulama (.appx) dosyalarıyla hızlı bir şekilde doluyor olabilir. Bu sorunu çözmek için Microsoft Store’u sıfırlayın, Microsoft Store önbelleğini temizleyin ve ardından Windows Update sorun gidericisini çalıştırın. Bu adımlara geçmeden önce Microsoft Store’un kapalı olduğundan emin olun.

**1. Adım: Microsoft Store’u sıfırlayın**

**Not** Bu işlem, tercihleriniz ve oturum açma bilgileriniz dahil olmak üzere cihazdaki uygulama verilerini kalıcı olarak siler.

1. **Başlat** > **Ayarlar** > **Uygulamalar** > **Uygulamalar ve özellikler**’i seçin.

1. Uygulamalar listesinde Microsoft Store’u bularak seçin.

1. **Gelişmiş seçenekler**’i seçin.

1. Aşağı kaydırın, **Sıfırla**’yı ve ardından **Sıfırlamayı Onayla** yı seçin.

**2. Adım: Microsoft Store önbelleğini temizleyin**

1. Windows logo tuşu + R tuşlarına basarak Çalıştır iletişim kutusunu açın.

1. Kutuya wsreset.exe yazın ve **Tamam**’ı seçin.

1. Boş bir Komut İstemi penceresi açılır. Yaklaşık 10 saniye sonra pencere kapanır ve Microsoft Store otomatik olarak açılır.

**3. Adım: Windows Update’i sıfırlayın**

1. **Başlat** > **Ayarlar** > **Güncelleştirme ve Güvenlik** > **Sorun giderme**’yi seçin.

1. Aşağı kaydırın ve listeden **Windows Update**’i seçin ve **Sorun gidericiyi çalıştır**’ı seçin.

1. Bilgisayarınızı yeniden başlatın ve sorunla karşılaşmaya devam edip etmediğinizi kontrol edin.

