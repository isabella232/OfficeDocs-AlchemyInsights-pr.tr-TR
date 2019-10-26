---
title: Outlook Desktop bir e-posta iletisi geri çağırma veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496131"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-posta iletisi geri çağırma veya değiştirme

- Yönetici olarak **PowerShell kullanan kullanıcılar adına iletileri geri çağırabilirsiniz.** Yönetici merkezinden gelen iletileri geri çağıramazsınız.
- Yalnızca **kuruluşunuzdaki kişilere gönderilen iletileri geri çağırabilirsiniz.** İleti bir Gmail adresine gönderildiyse, örneğin, iletiyi geri çağıramazsınız.
- Yalnızca **Outlook 2016'dan gönderilen iletileri pc'de hatırlayabilirsiniz.** Bir kullanıcı web'de Mac için Outlook veya Outlook kullanarak bir ileti gönderirse, bunu geri çağıramazsınız.

Bir e-posta iletisini geri çağırmak veya değiştirmek için:

1. Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.
1. Açmak için hatırlamak istediğiniz iletiyi çift tıklatın.
1. **İleti** sekmesini seçin ve ardından **Eylemler** > **Bu İletiyi Geri Çağır'ı**seçin.
1. **Bu iletinin okunmamış kopyalarını sil'i** seçin veya **okunmamış kopyaları silin ve yeni bir iletiyle değiştirin**ve ardından **Tamam'ı**seçin.
1. Yeni bir ileti gönderiyorsanız, iletiyi oluşturun ve sonra **Gönder'i**seçin.
1. İleti geri çağırmanın başarısı veya başarısızlığı, alıcının Outlook'taki ayarlarına bağlıdır. Geri çağırmayı denetlemek için adımlar için [bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.

Kuruluşunuzdaki e-posta iletilerini arama ve silme

- Genel bir yönetici değilseniz, iletileri aramak için hesabınızın eDiscovery Manager rolüne veya Uyumluluk Arama yönetimi rolüne eklenmesi gerekir. İletileri silmek için, Organizasyon Yönetimi rol grubuna veya Arama ve Temizleme yönetimi rolüne katılmanız gerekir. Bu rolleriçin izinler [Güvenlik ve uyumluluk merkezinde](https://go.microsoft.com/fwlink/?linkid=2083731)atanır.
- Silmek için ileti bulmak için [bir içerik araması oluşturun.](https://docs.microsoft.com/office365/securitycompliance/content-search)
- [Güvenlik ve Uyumluluk Merkezi PowerShell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Çok faktörlü kimlik doğrulama kullanıyorsanız, [çok faktörlü kimlik doğrulaması kullanarak Office 365 Güvenlik ve Uyumluluk Merkezi PowerShell'e bağlan'a](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bakın.