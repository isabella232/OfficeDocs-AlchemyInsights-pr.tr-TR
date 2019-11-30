---
title: Etkinleştirme Sorunu - Şu anda bağlanamıyoruz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628262"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office uygulamalarını düzeltme "Şu anda bağlanamıyoruz" iletisi

Bu iletiyi alırsanız, aşağıdakileri deneyin:

1. Office uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin. Bkz. [Office 365 URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. **Başlat** > **Çalıştır'a**gidin ve ardından **services.msc**yazın. Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:
    - Ağa Bağlı Cihazlar Otomatik Kurulum
    - Ağ Listesi Hizmeti
    - Ağ Konum Farkındalığı
    - Windows Etkinlik Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut bittikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Office 365'ten Office'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)