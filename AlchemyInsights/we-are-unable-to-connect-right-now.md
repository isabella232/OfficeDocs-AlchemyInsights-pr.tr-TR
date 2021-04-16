---
title: Etkinleştirme Sorunu - Şu anda bağlanaayız
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806462"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 uygulamalarını düzeltme "Şu anda bağlanalarız" iletisi

Bu iletiyi alırsanız, şunları deneyin:

1. Güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin ve Microsoft 365 uygulamalarına İnternet erişimini engellemelerini engellemez. Bkz. [Microsoft URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Başlangıç **Çalıştırma'ya**  >  **gidin** ve **services.msc yazın.** Aşağıdaki hizmetlerin hepsinin çalıştırlı olduğundan emin olun:
    - Ağ Bağlantılı Cihazlar Otomatik Kurulumu
    - Ağ Listesi Hizmeti
    - Ağ Konumu Farkındalığı
    - Windows Olay Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmayla ilgili bir sorun varsa yükseltilmiş izinlerle bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut tamamdikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz. "Ne üzgünüz, hesabınıza bağlana üzgünüz. Office'i Microsoft 365'den etkinleştirirken lütfen daha sonra yeniden deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)