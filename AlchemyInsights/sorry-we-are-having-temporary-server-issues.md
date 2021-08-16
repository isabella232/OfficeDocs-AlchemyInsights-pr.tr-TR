---
title: Geçici Microsoft 365 sorunlarını giderme Ne üzgünüz, geçici sunucu sorunları iletisiyle karşıda
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021616"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Aşağıdaki Microsoft 365 "Ne üzgünüz, geçici sunucu sorunlarımız var" iletisi

Bu iletiyi alırsanız, şunları deneyin:

1. Güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin ve bu uygulamaların İnternet erişimini engelleme Microsoft 365 yapın. Bkz. [URL'ler ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Başlangıç **Çalıştırma'ya**  >  **gidin** ve **services.msc yazın.** Aşağıdaki hizmetlerin hepsinin çalıştırlı olduğundan emin olun:
    - Ağ Bağlantılı Cihazlar Otomatik Kurulumu
    - Ağ Listesi Hizmeti
    - Ağ Konumu Farkındalığı
    - Windows Olay Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmayla ilgili bir sorun varsa yükseltilmiş izinlerle bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut tamamdikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz. "Ne üzgünüz, hesabınıza bağlana üzgünüz. 'i etkinleştirirken lütfen daha sonra yeniden deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)