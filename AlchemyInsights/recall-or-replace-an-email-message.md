---
title: E-posta iletisi geri çekme veya değiştirme
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024406"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-posta iletisinizi geri çekme veya değiştirme Microsoft 365

- Yalnızca **kuruluşun kişilerine gönderilen iletileri geri çağırabilirsiniz.** Örneğin, ileti bir Gmail adresine gönderildiyse, geri çağırasınız.
- Yalnızca **BILGISAYARıNıZ için bir Outlook gönderilen iletileri geri çağırabilirsiniz.** Kullanıcı e-posta Mac için Outlook Web üzerinde Outlook ileti gönderirse, iletiyi geri çağırasınız.
- Kiracı yöneticisi olarak, **PowerShell** kullanarak kullanıcıların adına iletileri geri çağırabilirsiniz (Daha fazla bilgi için bkz. E-posta iletilerini arama [ve silme).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Yönetim merkezinden gelen iletileri geri çağırasınız. Daha fazla bilgi için ekranı aşağı kaydırarak "Kuruluş içinde e-posta iletilerini arama ve silme" ifadesinin yer alır.

**Gönderdiniz e-posta iletisi geri çekme veya değiştirme**

1. Yeni Klasör penceresinin sol klasör Outlook Gönderilmiş Öğeler klasörünü seçin.
2. Geri çağırmak istediğiniz iletiyi açın. İletiyi açmak için çift tıklamanız gerekir. İletinin okuma bölmesinde iletiyi geri çekmesine izin vermez.
3. İleti sekmesinde, Bu İletiyi Geri **Çekme Eylemleri**  >  **öğesini seçin.**
4. Bu **iletinin okunmamış kopyalarını sil'i veya Okunmamış** kopyaları sil ve yerine yeni bir ileti **gönder'i,** sonra da Tamam'ı **seçin.**
5. Yeni bir ileti gönderiyorsanız, iletiyi yazın ve Gönder'i **seçin.**
6. Bir geri çağırmanın başarılı veya başarısızlığı alıcının geri çekme ayarlarına Outlook.

Geri çekmenin nasıl iade edildi olduğu da dahil olmak üzere daha fazla bilgi için bkz. [Gönderdiğiniz e-posta mesajını geri](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)çekme veya değiştirme .

***En kolay yol, kuruluş içinde e-posta*** iletilerini aramak ve silmektir; bu en kolayı genel yöneticiyseniz yapmaktır. Genel yönetici değilseniz, hesabınız eBulma Yöneticisi rol grubuna veya Uyumluluk Arama yönetimi rolüne eklenmiştir. İletileri silmek için, Kuruluş Yönetimi rol grubuna veya Arama ve Temizleme yönetim rolüne katılmanız gerekir. Bu rollere izinler Güvenlik ve [Uyumluluk & atanır.](https://protection.office.com/)

1. [Silinecek iletiyi](https://docs.microsoft.com/microsoft-365/compliance/content-search) bulmak için içerik araması oluşturun.
2. [Bağlan ve Uyumluluk & PowerShell'e.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

MFA (çok faktörlü kimlik doğrulaması) kullanıyorsanız, [Multi-Factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)Authentication Bağlan Güvenlik Microsoft 365 & PowerShell'i kullanmaya devam edin.
