---
title: E-posta iletisi geri çağırma veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509476"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Microsoft 365'te bir e-posta iletisi geri çağırma veya değiştirme

- Yalnızca **kuruluşunuzdaki kişilere gönderilen iletileri geri çağırabilirsiniz.** İleti bir Gmail adresine gönderildiyse, örneğin, iletiyi geri çağıramazsınız.
- Yalnızca **PC için Outlook 2016'dan gönderilen iletileri geri çağırabilirsiniz.** Bir kullanıcı web'de Mac için Outlook veya Outlook kullanarak bir ileti gönderirse, bunu geri çağıramazsınız.
- Yöneticiyseniz, **PowerShell'i kullanarak kullanıcılar adına iletileri geri çağırabilirsiniz.** Yönetici merkezinden gelen iletileri geri çağıramazsınız. Daha fazla bilgi için "Kuruluşunuzdaki e-posta iletilerini arayın ve silin" olarak aşağı kaydırın.

**Gönderdiğiniz bir e-posta iletisi geri çağırma veya değiştirme**

1. Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.
2. Hatırlamak istediğiniz iletiyi açın. İletiyi açmak için çift tıklatmanız gerekir. İletinin okuma bölmesinde görünmesi için seçilmesi, iletiyi geri çağırmanıza izin vermez.
3. İleti sekmesinden, **Eylemler**  >  **Bu İletiyi Geri Çağır'ı**seçin.
4. **Bu iletinin okunmamış kopyalarını sil'i** seçin veya **okunmamış kopyaları silin ve yeni bir iletiyle değiştirin,** ardından **Tamam'ı**seçin.
5. Yeni bir ileti gönderiyorsanız, iletiyi oluşturun ve **gönder'i**seçin.
6. İleti geri çağırmanın başarısı veya başarısızlığı, Alıcıların Outlook'taki ayarlarına bağlıdır.

Geri çağırmayı nasıl denetleyeceksiniz gibi daha fazla bilgi [için, gönderdiğiniz bir e-posta iletisini geri çağır'a bakın veya değiştirin.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Kuruluşunuzdaki e-posta iletilerini arama ve silme*** Kuruluşunuzdaki e-posta iletilerini aramak ve silmek için, genel bir yöneticiyseniz en kolayı buolur. Genel bir yönetici değilseniz, hesabınızın eDiscovery Manager rol grubuna veya Uyumluluk Arama yönetimi rolüne eklenmesi gerekir. İletileri silmek için, Organizasyon Yönetimi rol grubuna veya Arama ve Temizleme yönetimi rolüne katılmanız gerekir. Bu rollere ait izinler [Güvenlik & uyumluluk merkezinde](https://protection.office.com/)atanır.

1. Silmek için ileti bulmak için [bir içerik araması oluşturun.](https://docs.microsoft.com/microsoft-365/compliance/content-search)
2. [Güvenlik & Uyumluluk Merkezi PowerShell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps) 

MFA kullanıyorsanız, çok [faktörlü kimlik doğrulaması kullanarak Microsoft 365 güvenlik & Uyumluluk Merkezi PowerShell'e bağlan'a](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bakın. 
