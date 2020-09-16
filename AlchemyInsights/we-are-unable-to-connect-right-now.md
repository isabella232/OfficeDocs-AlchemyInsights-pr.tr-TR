---
title: Etkinleştirme sorunu-şu an bağlantı kuramıyoruz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726003"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 uygulamalarını düzeltme "hemen bağlantı kuramıyoruz" iletisi

Bu iletiyi alırsanız, aşağıdakileri deneyin:

1. Güvenlik duvarınızın, virüsten koruma yazılımınızın ve proxy ayarlarınızın Internet erişimini Microsoft 365 uygulamalarına engellemediğinden emin olmak için denetleyin. [Microsoft URL 'leri ve IP adresi aralıklarını](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)görün.

2. Başlat 'ı **başlatın**  >  **Run**ve ardından **Services. msc**yazın. Aşağıdaki hizmetlerin tümünün çalıştığından emin olun:
    - Ağ bağlantılı cihazların otomatik kurulumu
    - Ağ listesi hizmeti
    - Ağ konumu tanıma
    - Windows olay günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatırken bir sorun yaşıyorsanız, yükseltilmiş izinlerle komut istemini açarak aşağıdaki komutu çalıştırabilirsiniz:

**sfc/scannow**

Bu komut bittiğinde bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için, [hesabınıza bağlanamıyoruz "Üzgünüz. Office 'i Microsoft 365 'i etkinleştirdiğinizde lütfen daha sonra tekrar deneyin](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).