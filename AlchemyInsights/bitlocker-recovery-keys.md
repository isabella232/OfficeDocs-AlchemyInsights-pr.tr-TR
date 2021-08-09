---
title: Bitlocker kurtarma anahtarları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060084"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker kurtarma anahtarlara erişme

Bitlocker ayarları Intune Kurtarma Endpoint Protection yapılandırılamazken, Bitlocker kurtarma bilgisinin daha önce depolanmış olup olmadığını Azure Active Directory.

Bu ayar yapılandırılmışsa, Intune Cihaz Blade'sinde cihaz kaydı verileri iki şekilde bir intune yöneticisi tarafından görülebilir:

Cihazlar - Azure AD cihazlar ->" VEYA Cihazlar -> Tüm Cihazlar ->" -> Kurtarma anahtarları

Alternatif olarak, cihazın kendisine yönetim erişimi varsa, yükseltilmiş komut isteminden aşağıdaki komut çalıştırarak kurtarma anahtarı (Parola) görülebilir:

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
Cihaz Intune'da işlenmeden önce şifrelenmişse, kurtarma anahtarı OOBE işlemi sırasında cihazda oturum aparken kullanılan "Microsoft Hesabı" (MSA) ile ilişkilendirilmiş olabilir. Böyle bir durumda, MSA'ya erişme ve bu MSA ile oturum açma, kurtarma  https://onedrive.live.com/recoverykey anahtarlarının depolandığı cihazları gösterir.
 
Etki alanı tabanlı grup ilkesi aracılığıyla yapılandırma sonucunda cihaz şifrelenirse, kurtarma bilgileri şirket içi Active Directory'de depolanıyor olabilir.

Kurtarma anahtarını Azure Active Directory'de depolamak için uç nokta koruma ilkesi yapılandırdınız ancak belirli bir cihazın anahtarı karşıya yüklenmedi ise, bu cihaz için kurtarma anahtarını MEM konsolundan döndürerek karşıya yüklemenin tetiklenir. Ayrıntılar için bkz. [BitLocker kurtarma anahtarlarını döndürme.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

