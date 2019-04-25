---
title: Outlook Masaüstü geri çağırma veya değiştirme bir e-posta iletisi
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389803"
---
# <a name="recall-or-replace-an-email-message"></a>Çağrılacağı ya da bir e-posta iletisi

- Yönetici, **PowerShell kullanan kullanıcılar adına ileti geri çekme**olabilir. Yönetim Merkezi iletilerden Çekemiyor.
- **Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri çağırma**kullanabilirsiniz. Örneğin, Gmail adresine ileti gönderilmişse, onu Çekemiyor.
- **Yalnızca PC'de 2016 Outlook uygulamasından gönderilen iletileri geri çağırma**kullanabilirsiniz. Bir kullanıcı Mac için Outlook veya Outlook Web kullanarak bir ileti gönderirse, Çekemiyor.

Çağrılacağı ya da bir e-posta iletisi için:

1. Gönderilmiş Öğeler klasörü Outlook penceresinin soldaki klasör bölmesinde seçin.
1. Açmak için geri çekmek istediğiniz iletiyi çift tıklatın.
1. **İleti** sekmesini seçin ve sonra **Eylemler**seçin > **Bu iletiyi Geri Çağır**.
1. **Bu iletinin okunmamış kopyalarını sil** veya **Okunmamış kopyaları sil ve yerine yeni iletiler koy**seçin ve **Tamam**' ı seçin.
1. Yeni ileti gönderiyorsanız, iletinizi oluşturun ve **Gönder**' i seçin.
1. Başarı veya başarısızlık ileti geri çağırma alıcının Outlook ayarlarına bağlıdır. Geri çekme üzerinde denetlemek adımlar için [Bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.

Arama ve kuruluşunuzdaki e-posta iletilerini silme

- Genel Yönetici değilseniz, eBulma Yöneticisi rolü veya uyumluluk arama yönetimi rolü için iletileri aramak için hesabınıza eklenmesi gerekir. İletileri silmek için Kuruluş Yönetimi rol grubunun ya da arama ve temizleme yönetim rolü katılmak gerekir. Bu roller için izinleri [Güvenlik ve Uyumluluk Merkezi](https://go.microsoft.com/fwlink/?linkid=2083731)atanır.
- İletiyi silmek için bulmak için [arama içerik oluşturma](https://docs.microsoft.com/office365/securitycompliance/content-search) .
- [Güvenlik ve Uyumluluk Merkezi PowerShell bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Çok faktörlü kimlik doğrulaması kullanıyorsanız, [çok faktörlü kimlik doğrulama kullanarak bağlan Office 365 güvenlik ve Uyumluluk Merkezi PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bakın.