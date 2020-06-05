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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581895"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 uygulamalarını düzeltme "Şu anda bağlanamıyoruz" iletisi

Bu iletiyi alırsanız, aşağıdakileri deneyin:

1. Microsoft 365 uygulamalarına Internet erişimini engellemediklerini doğrulamak için güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin. [Bkz. Microsoft URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Başlat **Start**  >  **Çalıştır'a**gidin ve ardından **services.msc**yazın. Aşağıdaki hizmetlerin tümlerinin çalıştığını unutmayın:
    - Ağa Bağlı Cihazlar Otomatik Kurulum
    - Ağ Listesi Hizmeti
    - Ağ Konum Farkındalığı
    - Windows Etkinlik Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmakta sorun varsa, yüksek izinleri olan bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut bittikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz: "Üzgünüz, hesabınıza bağlanabiliyoruz. Microsoft 365'ten Office'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)