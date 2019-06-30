---
title: Çağrılacağı ya da bir e-posta iletisi
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356617"
---
# <a name="recall-or-replace-an-email-message"></a>Çağrılacağı ya da bir e-posta iletisi

- **Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri çağırma**kullanabilirsiniz. Örneğin, Gmail adresine ileti gönderilmişse, onu Çekemiyor.
- **Yalnızca PC için 2016 Outlook uygulamasından gönderilen iletileri geri çağırma**kullanabilirsiniz. Bir kullanıcı Mac için Outlook veya Outlook Web kullanarak bir ileti gönderirse, Çekemiyor.
- Bir yönetici iseniz, **PowerShell kullanarak kullanıcılar adına ileti geri çekme**olabilir. Yönetim Merkezi iletilerden Çekemiyor. "Ara ve kuruluşunuzdaki e-posta iletileri silme" daha fazla bilgi için gidin.

***Çağrılacağı ya da size gönderilen bir e-posta iletisi***

1. Gönderilmiş Öğeler klasörü Outlook penceresinin soldaki klasör bölmesinde seçin.
2. Geri çekmek istediğiniz iletiyi açın. İletiyi açmak için çift tıklatmanız gerekir. Okuma Bölmesi'nde görüntülenir, böylece iletiyi seçerek iletiyi geri çekmek izin vermiyor.
3. İleti sekmesinde, **Eylemler**seçin > **Bu iletiyi Geri Çağır**.
4. **Bu iletinin okunmamış kopyalarını sil** veya **Okunmamış kopyaları sil ve yerine yeni iletiler koy**seçin, sonra **Tamam**' ı seçin.
5. Değiştirme ileti gönderiyorsanız, iletinizi oluşturun ve **Gönder**' i seçin.
6. Başarı veya başarısızlık ileti geri çağırma Outlook alıcıları ayarlarına bağlıdır.

Geri çekme üzerinde nasıl kontrol edileceğini de dahil olmak üzere daha fazla bilgi için bkz: [geri çağırma veya değiştirme size gönderilen bir e-posta iletisi](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Arama ve kuruluşunuzdaki e-posta iletileri silme*** Genel yönetici iseniz aramak ve kuruluşunuzdaki e-posta iletilerini silmek için en kolay yöntemdir Genel Yönetici değilseniz, hesabınızı uyumluluğu arama yönetim rolü veya eBulma Yöneticisi Rol grubuna eklenmesi gerekir. İletileri silmek için Kuruluş Yönetimi rol grubunun ya da arama ve temizleme yönetim rolü katılmak gerekir. [Güvenlik & Uyumluluk Merkezi](https://protection.office.com/)bu rollere izinler atanır.

1. İletiyi silmek için bulmak için [arama içerik oluşturma](https://docs.microsoft.com/office365/securitycompliance/content-search) .
2. [Güvenlik & Uyumluluk Merkezi PowerShell için bağlayın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

MFA kullanıyorsanız, [çok faktörlü kimlik doğrulama kullanarak bağlan Office 365 güvenlik & Uyumluluk Merkezi PowerShell için](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bkz. 
