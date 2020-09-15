---
title: Outlook masaüstü bir e-posta iletisini geri çekme veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664010"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-posta iletisini geri çekme veya değiştirme

- Yönetici olarak, **PowerShell kullanarak kullanıcıları adına iletileri geri çekbırakabilirsiniz**. Yönetim merkezinden iletileri geri çekemezsiniz.
- **Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri**yükleyebilirsiniz. Örneğin, ileti gmail adresine gönderildiyse, geri çekilemiyor.
- **Bilgisayarda yalnızca Outlook 2016 tarafından gönderilen iletileri geri çekmeniz**yeterlidir. Bir Kullanıcı, Mac için Outlook veya Web üzerinde Outlook kullanan bir ileti gönderirse, geri çekemezsiniz.

E-posta iletisini geri çekmek veya değiştirmek için:

1. Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.
1. Geri çekmek istediğiniz iletiye çift tıklayarak açın.
1. **İleti** sekmesini ve sonra da eylemler 'i seçin **Actions**  >  **Recall This Message**.
1. **Bu iletinin okunmamış kopyalarını sil** 'i veya **Okunmamış kopyaları sil**'i seçin ve sonra da **Tamam 'ı**seçin.
1. Değiştirme iletisi gönderiyorsanız iletiyi oluşturun ve **Gönder**'i seçin.
1. İletinin geri çekme başarısı veya başarısızlığı, alıcının Outlook 'taki ayarlarına bağlıdır. Geri çekmeyi denetleme adımları için [Bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.

Kuruluşunuzdaki e-posta iletilerini arama ve silme

- Genel yönetici değilseniz, hesap aramak için hesabınızın eBulma Yöneticisi rolüne veya uyumluluk arama yönetimi rolüne eklenmesi gerekir. İletileri silmek için, Kuruluş Yönetimi rol grubuna veya arama ve Temizleme Yönetim rolüne katılmanız gerekir. Bu rollerin izinleri [güvenlik ve Uyumluluk Merkezi](https://go.microsoft.com/fwlink/?linkid=2083731)'nde atanır.
- Silinecek iletiyi bulmak için [içerik araması oluşturun](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
- [Güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Multi-Factor Authentication kullanıyorsanız, [Multi-Factor Authentication kullanarak Microsoft 365 güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).