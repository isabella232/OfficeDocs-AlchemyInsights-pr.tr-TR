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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628010"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi

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