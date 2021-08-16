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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998192"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Şu Microsoft 365 düzeltme "Şu anda bağlanalarız" iletisi

Bu iletiyi alırsanız, şunları deneyin:

1. Güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin ve bu uygulamaların İnternet erişimini engelleme Microsoft 365 yapın. Bkz. [Microsoft URL'leri ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Başlangıç **Çalıştırma'ya**  >  **gidin** ve **services.msc yazın.** Aşağıdaki hizmetlerin hepsinin çalıştırlı olduğundan emin olun:
    - Ağ Bağlantılı Cihazlar Otomatik Kurulumu
    - Ağ Listesi Hizmeti
    - Ağ Konumu Farkındalığı
    - Windows Olay Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmayla ilgili bir sorun varsa yükseltilmiş izinlerle bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut tamamdikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz. "Ne üzgünüz, hesabınıza bağlana üzgünüz. Office etkinleştirme sırasında lütfen daha sonra yeniden Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)