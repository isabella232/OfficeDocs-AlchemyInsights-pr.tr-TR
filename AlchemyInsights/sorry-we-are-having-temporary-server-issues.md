---
title: Office uygulamalarını düzeltmeÜzgünüz, geçici sunucu sorunları iletisi alıyoruz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764137"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi

Bu iletiyi alırsanız, aşağıdakileri deneyin:

1. Office uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin. [URL'lere ve IP adres aralıklarına](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)bakın.

2. **Başlat** > **Çalıştır'a**gidin ve ardından **services.msc**yazın. Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:
    - Ağa Bağlı Cihazlar Otomatik Kurulum
    - Ağ Listesi Hizmeti
    - Ağ Konum Farkındalığı
    - Windows Etkinlik Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut bittikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Lütfen daha sonra tekrar deneyin" hatanızı etkinleştirdiğinizde.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)