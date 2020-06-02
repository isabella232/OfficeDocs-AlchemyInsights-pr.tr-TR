---
title: Microsoft 365 2681 Saldırı Simülatörü
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506758"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365'te Saldırı Simülatörü

- Saldırı Simülatörü'nü kaçırıyor musunuz? Saldırı Simülatörü **Office 365 Gelişmiş Tehdit Koruma Planı 2 (ATP Planı 2)** veya **Office 365 Enterprise E5**gerektirir. Saldırı Simülasyon Aracı, Office 365 Gelişmiş Tehdit Koruma Planı 1 (ATP Plan 1), Office 365 Enterprise E3 veya iş abonelikleri için herhangi bir Microsoft 365 Sürümüne dahil **değildir.**

- Benzetimli saldırılar başlatmak için kullandığınız hesap, genel yönetici veya güvenlik yöneticisi izinleri ve çok faktörlü kimlik doğrulama (MFA) gerektirir. Saldırı Simülatörü gereksinimleri hakkında daha fazla bilgi için [bu konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.

- **Brute Force Password** saldırı simülasyonları hakkında bilinmesi gereken önemli şeyler:

  - Hedef hesap MFA etkinleştirilmişse ve parola doğru tahmin edildiyse, hesap tehlikeye atılmış olarak gösterilmez (ikinci kimlik doğrulama faktörü eksik olur).

  - Parola dosyası 10 MB'dan büyük olamaz. Satır başına bir parola kullanın ve listedeki son paroladan sonra boş bir satır (satır başı) ekleyin.

- **Spear Phishing** hakkında bilinmesi gereken önemli şeyler simülasyonları ekleyin:

  - Tasarım gereği, **Kimlik Avı giriş sunucusu URL'si**için özel bir değer sağlayamaz.

  - Bir alıcı, [iletiyi](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kimlik avı olarak bildirmek için Rapor İletisi eklentisini etkinleştir'i kullanırsa, ileti için uyarı almayabilirsiniz (bu simüle edilmiş bir saldırı olduğu için).

- Raporlar: Benzetimli saldırı tamamlandıktan sonra, raporu görmek için **Saldırı Ayrıntıları'nı** tıklatabilirsiniz.

- Attack Simulator'daki ayrıntılı talimatlar ve yeni özellikler için [Microsoft 365'teki Saldırı Simülatörü'ne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.
