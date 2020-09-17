---
title: E-posta iletisini geri çekme veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799224"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Microsoft 365 'de e-posta iletisini geri çekme veya değiştirme

- **Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri**yükleyebilirsiniz. Örneğin, ileti gmail adresine gönderildiyse, geri çekilemiyor.
- **PC Için Outlook 2016 ' den gönderilen iletileri geri çekmeniz**yeterlidir. Bir Kullanıcı, Mac için Outlook veya Web üzerinde Outlook kullanan bir ileti gönderirse, geri çekemezsiniz.
- Yöneticiyseniz, **PowerShell kullanarak iletileri Kullanıcı adına geri çekbırakabilirsiniz**. Yönetim merkezinden iletileri geri çekemezsiniz. Daha fazla bilgi için "kuruluşunuzdaki e-posta iletilerini arayın ve silin" için aşağı kaydırın.

**Gönderdiğiniz e-posta iletisini geri çekme veya değiştirme**

1. Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.
2. Geri çekmek istediğiniz iletiyi açın. İletiyi açmak için çift tıklatın. İletiyi, okuma bölmesinde görünecek şekilde seçmek iletiyi geri çekmenizi sağlar.
3. İleti sekmesinden, **Actions**  >  **Bu iletiyi geri çek**eylemler 'i seçin.
4. **Bu iletinin okunmamış kopyalarını sil** 'i veya **Okunmamış kopyaları sil 'i seçin ve yeni bir iletiyle değiştirin**, ardından **Tamam 'ı**seçin.
5. Değiştirme iletisi gönderiyorsanız iletiyi oluşturun ve **Gönder**'i seçin.
6. İletinin geri çekme başarısı veya başarısızlığı, alıcıların Outlook 'taki ayarlarına bağlıdır.

Geri çekmeyi denetleme dahil olmak üzere daha fazla bilgi için, [gönderdiğiniz e-posta Iletisini geri çekme veya değiştirme](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)konusuna bakın.

***Kuruluşunuzdaki e-posta Iletilerini arama ve silme*** Kuruluşunuzdaki e-posta iletilerini aramak ve silmek için, genel bir yönetici olmanız en kolay yoldur. Genel yönetici değilseniz, hesabınız eBulma Yöneticisi rol grubuna veya uyumluluk arama yönetimi rolüne eklenmelidir. İletileri silmek için, Kuruluş Yönetimi rol grubuna veya arama ve Temizleme Yönetim rolüne katılmanız gerekir. Bu rollerin izinleri [güvenlik & Uyumluluk Merkezi](https://protection.office.com/)'nde atanır.

1. Silinecek iletiyi bulmak için [içerik araması oluşturun](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
2. [Güvenlik & Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

MFA kullanıyorsanız, [Multi-Factor Authentication kullanarak Microsoft 365 güvenlik & Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
