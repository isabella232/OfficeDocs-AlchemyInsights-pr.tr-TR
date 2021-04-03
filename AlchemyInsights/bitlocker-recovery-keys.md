---
title: Bitlocker kurtarma anahtarları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505088"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker kurtarma tuşlarına erişme

Bitlocker ayarlarını Intune Uç Nokta Koruma İlkesi yapılandırarak Bitlocker kurtarma bilgisinin Azure Active Directory'de depolanmış olup olmadığını tanımlamak mümkündür.

Bu ayar yapılandırılmışsa, Intune Devices blade'te cihaz kaydı verileri iki şekilde bir intune yöneticisi tarafından görülebilir:

Cihazlar - Azure AD cihazları -> "Cihaz" VEYA Cihazlar -> Tüm Cihazlar -> "Cihaz" -> Kurtarma anahtarları

Alternatif olarak, cihazın kendisine yönetim erişimi varsa, yükseltilmiş komut isteminden aşağıdaki komutu çalıştırarak kurtarma anahtarı (Parola) görülebilir:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Cihaz Intune'da şifrelenmeden önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında cihazda oturum a açmada kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir. Böyle bir durumda, MSA'ya erişme ve bu MSA ile oturum açma, kurtarma  https://onedrive.live.com/recoverykey anahtarlarının depolandığı cihazları gösterir.
 
Cihaz, etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda şifrelenirse, kurtarma bilgileri şirket içi Active Directory'de depolanıyor olabilir.

Kurtarma anahtarını Azure Active Directory'de depolamak için Uç Nokta koruma ilkesi yapılandırdınız ancak belirli bir cihaza yönelik anahtar karşıya yüklenmedi ise, mem konsolundan bu cihazın kurtarma anahtarını döndürerek karşıya yüklemenin tetiklenir. Ayrıntılar için bkz. [BitLocker kurtarma anahtarlarını döndürme.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

