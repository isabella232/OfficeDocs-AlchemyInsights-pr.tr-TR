---
title: 2681 saldırı Simülat365 örü
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801571"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365 'de saldırı simülatörü

- Saldırı simülatörü eksik mısınız? Saldırı simülatörü **Için Microsoft Defender for Office 365 Plan 2 (ATP plan 2)** veya **Office 365 Kurumsal E5** . Saldırı simülatörü, Office 365 plan 1 (ATP planı 1), Office 365 Kurumsal E3 veya iş abonelikleri için 365 Microsoft Defender 'a dahil **değildir** .

- Benzetilmiş saldırıları başlatmak için kullandığınız hesap, genel yönetici veya Güvenlik Yöneticisi izinleri ve çok faktörlü kimlik doğrulaması (MFA) gerektirir. Saldırı simülatörü gereksinimleri hakkında daha fazla bilgi için [Bu konuya](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)bakın.

- **Kaba, parola** saldırısı benzetimleri ile ilgili bilinmesi gereken önemli noktalar:

  - Hedef hesaba MFA etkinleştirilmişse ve parola doğru tahmindiyse, hesap tehlikeye düşmesi halinde gösterilmez (ikinci kimlik doğrulama faktörü tamamlanmamış olacaktır).

  - Parola dosyası 10 MB 'den büyük olamaz. Her satırda bir parola kullanın ve listedeki son parolanın sonrasına boş bir satır (satır başı) ekleyin.

- **Spear sızdırma** ile ilgili bilinmesi gereken önemli noktalar:

  - Tasarıma göre, **kimlik avı oturum sunucusu URL 'si** için özel bir değer sağlayamıyoruz.

  - Alıcı, iletiyi kimlik avı olarak bildirmek için [rapor ileti eklentisini etkinleştir](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) seçeneğini kullanırsa, ileti için uyarı alamayabilirsiniz (Bu, benzetilmiş bir saldırı nedeniyle).

- Raporlar: benzetim işlemi tamamlandıktan sonra, raporu görmek için **saldırı ayrıntıları** 'na tıklayabilirsiniz.

- Saldırı [365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)simülatörü ile ilgili ayrıntılı yönergeler ve yeni özellikler
