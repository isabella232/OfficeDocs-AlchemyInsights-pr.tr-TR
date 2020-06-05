---
title: Microsoft 365 uygulamaları sabitleme Üzgünüz, biz geçici sunucu sorunları mesajı yaşıyorsanız
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582723"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 uygulamalarını düzeltme "Üzgünüz, geçici sunucu sorunları yaşıyoruz" iletisi

Bu iletiyi alırsanız, aşağıdakileri deneyin:

1. Microsoft 365 uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin. [URL'lere ve IP adres aralıklarına](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)bakın.

2. Başlat **Start**  >  **Çalıştır'a**gidin ve ardından **services.msc**yazın. Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:
    - Ağa Bağlı Cihazlar Otomatik Kurulum
    - Ağ Listesi Hizmeti
    - Ağ Konum Farkındalığı
    - Windows Etkinlik Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut bittikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Lütfen daha sonra tekrar deneyin" hatanızı etkinleştirdiğinizde.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)