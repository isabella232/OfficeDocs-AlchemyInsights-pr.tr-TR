---
title: Outlook Masaüstü geri çekme veya e-posta iletisi değiştirme
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918415"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Bir e-posta Outlook geri çekme veya değiştirme

- Yönetici olarak, **PowerShell kullanan kullanıcılar adına iletileri geri çağırabilirsiniz.** Yönetim merkezinden gelen iletileri geri çağırasınız.
- Yalnızca **kuruluşun kişilerine gönderilen iletileri geri çağırabilirsiniz.** Örneğin ileti bir Gmail adresine gönderilmişse, geri çağırasınız.
- Yalnızca **PC'niz üzerinden Outlook 2016 iletileri geri çağırabilirsiniz.** Kullanıcı e-posta Mac için Outlook Web üzerinde Outlook ileti gönderirse, iletiyi geri çağırasınız.

E-posta iletisi geri çağırma veya değiştirme:

1. Dosya penceresinin sol klasör Outlook Gönderilmiş Öğeler klasörünü seçin.
1. Açmak için geri almak istediğiniz iletiyi çift tıklatın.
1. İleti sekmesini **seçin ve** sonra da Bu İletiyi Geri **Çekme Eylemleri** öğesini  >  **seçin.**
1. Bu **iletinin okunmamış kopyalarını sil'i veya Okunmamış** kopyaları sil ve yerine yeni bir ileti **gönder'i seçin** ve ardından Tamam'ı **seçin.**
1. Yeni bir ileti gönderiyorsanız, iletiyi yazın ve gönder'i **seçin.**
1. Bir geri çağırmanın başarılı veya başarısızlığı alıcının geri çekme ayarlarına Outlook. Geri çekme adımlarını denetleme adımları için bu [makaleye bakın.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Organizasyonda e-posta iletilerini arama ve silme

- Genel yönetici değilseniz, iletileri aramak için hesabınız eBulma Yöneticisi rolüne veya Uyumluluk Arama yönetimi rolüne eklenmiştir. İletileri silmek için, Kuruluş Yönetimi rol grubuna veya Arama ve Temizleme yönetim rolüne katılmanız gerekir. Bu rollerin izinleri Güvenlik ve uyumluluk [merkezinden atanır.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Silinecek iletiyi](https://docs.microsoft.com/microsoft-365/compliance/content-search) bulmak için içerik araması oluşturun.
- [Bağlan ve Uyumluluk Merkezi PowerShell'e.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Çok faktörlü kimlik doğrulaması kullanıyorsanız, [multi-factor authentication Bağlan PowerShell Microsoft 365 i](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)yeniden kullanmak için bkz.